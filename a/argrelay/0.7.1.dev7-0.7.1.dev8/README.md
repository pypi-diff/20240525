# Comparing `tmp/argrelay-0.7.1.dev7.tar.gz` & `tmp/argrelay-0.7.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argrelay-0.7.1.dev7.tar", last modified: Sat May 25 02:54:25 2024, max compression
+gzip compressed data, was "argrelay-0.7.1.dev8.tar", last modified: Sat May 25 03:15:57 2024, max compression
```

## Comparing `argrelay-0.7.1.dev7.tar` & `argrelay-0.7.1.dev8.tar`

### file list

```diff
@@ -1,417 +1,417 @@
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.348390 argrelay-0.7.1.dev7/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2024-05-19 10:16:55.000000 argrelay-0.7.1.dev7/LICENSE
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-05-25 02:54:25.348390 argrelay-0.7.1.dev7/PKG-INFO
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.308390 argrelay-0.7.1.dev7/docs/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.311390 argrelay-0.7.1.dev7/docs/dev_notes/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5535 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/docs/dev_notes/bootstrap_procedure.1.project_creation.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2509 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1924 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/dev_notes/brief_history.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2781 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/dev_notes/code_style.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev7/docs/dev_notes/completion_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6986 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/dev_notes/completion_perf_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/dev_notes/gui_tests_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5196 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/dev_notes/how_search_works.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2495 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/dev_notes/library_vs_framework.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/dev_notes/mongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1469 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/docs/dev_notes/next_steps_tutorial.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3776 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/dev_notes/origin_story.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7809 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/dev_notes/query_perf_10_x_more_data_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7149 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/dev_notes/query_perf_cache_vs_no_cache.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4285 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/dev_notes/query_perf_mongomock_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8388 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/dev_notes/query_perf_pymongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev7/docs/dev_notes/release_procedure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      769 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/dev_notes/screencast_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      787 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/docs/dev_notes/scripts_summary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1128 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/docs/dev_notes/semver_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5697 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/docs/dev_notes/term_dictionary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11129 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/dev_notes/top_todos.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3241 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/dev_notes/version_format.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.317390 argrelay-0.7.1.dev7/docs/feature_stories/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3725 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_00_13_77_97.plugin_framework.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_01_89_09_24.interp_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      778 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2912 2024-04-21 14:23:13.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      228 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1839 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      994 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      770 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_14_59_14_06.pending_requests.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1130 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_15_79_76_85.line_processor.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1476 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1028 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      761 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_20_88_05_60.named_args.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1914 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      917 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_26_43_73_72.func_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_27_16_67_19.line_syntax.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3596 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_29_54_67_86.dir_structure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1029 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_31_70_49_15.search_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      649 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_33_76_82_84.composite_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1829 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_36_17_84_44.check_env.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1764 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      849 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_39_58_01_91.query_cache.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1739 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1450 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_43_50_57_71.echo_args_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      792 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_46_96_59_05.init_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1278 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_47_63_35_61.env_vars.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1348 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1556 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_55_57_45_04.enum_selector.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2481 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1744 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_58_61_77_69.dev_shell.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      751 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1457 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_62_25_92_06.assigned_context.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1211 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_63_63_14_08.generated_config.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4075 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_66_17_43_42.test_infra.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2246 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_67_16_61_97.git_plugin.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1507 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_71_87_33_52.help_hint.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1916 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_72_40_53_00.fill_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_72_53_55_13.show_non_default_options.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_74_69_61_79.get_set_data_envelope.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1370 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      155 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_78_91_27_22.interp_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_80_45_89_81.integrated_functions.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2391 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2089 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4514 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      493 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1841 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1735 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_91_88_07_23.jump_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3287 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_92_75_93_01.clean_command_line.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_94_30_49_28.help_doc.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1653 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_97_64_39_94.arg_buckets.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      189 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_98_55_40_77.invoke_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      505 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/feature_stories/FS_99_81_19_25.no_space_in_options.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      454 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/feature_stories/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      637 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.318390 argrelay-0.7.1.dev7/docs/release_notes/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1240 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      165 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.0.0.dev0.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1368 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.0.0.dev27.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.0.0.dev28.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      133 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.0.0.dev42.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.0.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       37 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.1.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       98 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.2.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       75 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.2.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      124 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.3.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      273 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.4.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      328 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.5.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      136 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.5.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      245 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.5.2.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      403 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.6.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      411 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.6.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      110 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.6.2.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       62 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.6.3.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      143 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/release_notes/v0.6.4.final.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.321390 argrelay-0.7.1.dev7/docs/task_refs/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      573 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      336 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_04_84_79_11.reorganize_tests_for_CI.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      277 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_11_77_28_50.suggestions_in_all_responses.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      418 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_24_22_11_49.avoid_removing_last_history_command.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2979 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_26_15_31_78.categorize_git_repo_existence.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_27_61_22_18.make_shell_vars_local.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2661 2024-05-25 01:52:51.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_30_69_19_14.infinite_spinner.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      459 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_32_99_70_35.JSONPath_to_verify_response_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_37_15_12_91.Popen_mock.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      352 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_40_10_18_32.add_custom_base_to_all_schemas.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      349 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_43_41_95_86.use_server_logger_to_disable_stdout.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      560 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       85 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      703 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      497 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_all_packages_before_test.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      640 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      224 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_70_48_96_29.be_able_to_assert_remaining_arg_vals.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      422 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_75_52_01_67.arg_buckets_to_support_multiple_var_args.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      170 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_79_67_28_83.recursive_dict_schema.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      187 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      456 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      652 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3051 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      256 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/docs/task_refs/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.322390 argrelay-0.7.1.dev7/docs/test_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      695 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev7/docs/test_data/TD_38_03_48_51.large_data_set.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      387 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11158 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/test_data/TD_63_37_05_36.demo_services_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.7.1.dev7/docs/test_data/TD_70_69_38_46.no_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      550 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev7/docs/test_data/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.7.1.dev7/pyproject.toml
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15739 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2024-05-25 02:54:25.348390 argrelay-0.7.1.dev7/setup.cfg
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4262 2024-05-24 15:22:17.000000 argrelay-0.7.1.dev7/setup.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.306390 argrelay-0.7.1.dev7/src/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.322390 argrelay-0.7.1.dev7/src/argrelay/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev7/src/argrelay/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.323390 argrelay-0.7.1.dev7/src/argrelay/client_command_local/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1714 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_local/AbstractLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      997 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_local/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.323390 argrelay-0.7.1.dev7/src/argrelay/client_command_remote/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2304 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      857 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3981 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/client_command_remote/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.323390 argrelay-0.7.1.dev7/src/argrelay/client_spec/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3787 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/src/argrelay/client_spec/ShellContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/client_spec/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.324390 argrelay-0.7.1.dev7/src/argrelay/composite_tree/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      344 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeForest.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1138 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeForestSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2071 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeInfoType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1144 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeNode.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6371 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeNodeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      657 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeNodeType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13703 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeTreeWalker.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11778 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/composite_tree/DictTreeWalker.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/composite_tree/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.326390 argrelay-0.7.1.dev7/src/argrelay/custom_integ/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8164 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/BaseConfigDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2325 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/ConfigOnlyDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3643 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3533 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/ConfigOnlyLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1598 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1737 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/FuncConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1492 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8075 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1869 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12644 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1615 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      853 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/ServiceArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    18325 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/ServiceDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      217 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/ServiceEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    69098 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/ServiceLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      842 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2512 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/git_utils.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      413 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ/value_constants.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.327390 argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7009 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/argrelay_common_lib.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    33035 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     7248 2024-05-19 16:53:10.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/check_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     3390 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/dev_shell.bash
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3713 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/init_shell_env.bash
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8092 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/shell_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     2908 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/upgrade_all_packages.bash
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.328390 argrelay-0.7.1.dev7/src/argrelay/enum_desc/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1313 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/ArgSource.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1011 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/CallConv.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1498 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/CompScope.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2952 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/CompType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4670 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/DistinctValuesQuery.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/InterpStep.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      470 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/PluginType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      547 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/ReservedArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      190 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/ReservedEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1707 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/RunMode.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/ServerAction.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      390 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/SpecialChar.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      511 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/SpecialFunc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3091 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/TermColor.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1259 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/TokenType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev7/src/argrelay/enum_desc/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.329390 argrelay-0.7.1.dev7/src/argrelay/handler_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/src/argrelay/handler_request/AbstractServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      986 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3103 2024-04-22 16:25:28.000000 argrelay-0.7.1.dev7/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/handler_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.329390 argrelay-0.7.1.dev7/src/argrelay/handler_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      200 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/handler_response/AbstractClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9401 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1122 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1023 2024-04-13 16:33:00.000000 argrelay-0.7.1.dev7/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/handler_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.329390 argrelay-0.7.1.dev7/src/argrelay/misc_helper_common/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-05-18 02:28:39.000000 argrelay-0.7.1.dev7/src/argrelay/misc_helper_common/ElapsedTime.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      741 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/misc_helper_common/ObjectSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/misc_helper_common/TypeDesc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/src/argrelay/misc_helper_common/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.329390 argrelay-0.7.1.dev7/src/argrelay/misc_helper_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      521 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/misc_helper_server/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.330390 argrelay-0.7.1.dev7/src/argrelay/mongo_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev7/src/argrelay/mongo_data/MongoClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3649 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/mongo_data/MongoClientWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      616 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/mongo_data/MongoConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/mongo_data/MongoServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2086 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/mongo_data/MongoServerWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.1.dev7/src/argrelay/mongo_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.331390 argrelay-0.7.1.dev7/src/argrelay/plugin_config/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4367 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_config/AbstractConfigurator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4265 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_config/DefaultConfigurator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_config/DefaultConfiguratorConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1555 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_config/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.331390 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5958 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/AbstractDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4218 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/AbstractJumpDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1697 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/AbstractJumpDelegatorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2087 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/EchoDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1516 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/ErrorDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5791 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/HelpDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5308 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/InterceptDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      870 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/NoopDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1813 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/QueryEnumDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-08-06 08:09:50.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.333390 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3681 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/AbstractInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2278 2024-04-22 16:25:28.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/AbstractInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      701 2024-05-23 10:51:14.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FirstArgInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5508 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FirstArgInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1349 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    17429 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FuncTreeInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12865 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FuncTreeInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1684 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7238 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/InterpTreeInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6270 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/InterpTreeInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2925 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      384 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/NoopInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/NoopInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.333390 argrelay-0.7.1.dev7/src/argrelay/plugin_loader/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_loader/AbstractLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-12-14 14:18:48.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_loader/NoopLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/plugin_loader/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.334390 argrelay-0.7.1.dev7/src/argrelay/relay_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      965 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/relay_client/AbstractClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      366 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/relay_client/AbstractClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      266 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/relay_client/AbstractClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-10-21 04:19:27.000000 argrelay-0.7.1.dev7/src/argrelay/relay_client/RemoteClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1861 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/relay_client/RemoteClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.7.1.dev7/src/argrelay/relay_client/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2821 2024-05-25 02:19:11.000000 argrelay-0.7.1.dev7/src/argrelay/relay_client/__main__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4197 2024-05-25 02:19:11.000000 argrelay-0.7.1.dev7/src/argrelay/relay_client/proc_spinner.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2733 2024-05-25 02:19:11.000000 argrelay-0.7.1.dev7/src/argrelay/relay_client/proc_split.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2926 2024-05-25 01:48:26.000000 argrelay-0.7.1.dev7/src/argrelay/relay_client/proc_worker.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.335390 argrelay-0.7.1.dev7/src/argrelay/relay_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11191 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/CustomFlaskApp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/GuiBannerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1500 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/HelpHintCache.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7312 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/LocalServer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/QueryCacheConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13331 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/QueryEngine.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1147 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/QueryResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/__main__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.335390 argrelay-0.7.1.dev7/src/argrelay/relay_server/gui_static/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31127 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/gui_static/argrelay_client.js
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      318 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/gui_static/argrelay_favicon.ico
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4987 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/gui_static/argrelay_style.css
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/gui_static/external_link.svg
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.335390 argrelay-0.7.1.dev7/src/argrelay/relay_server/gui_templates/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7812 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/gui_templates/argrelay_main.html
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4947 2024-05-17 16:12:06.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/route_api.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1894 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/relay_server/route_gui.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.336390 argrelay-0.7.1.dev7/src/argrelay/runtime_context/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3180 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_context/AbstractPlugin.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4398 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_context/EnvelopeContainer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_context/InitControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    17397 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_context/InterpContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6354 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_context/ParsedContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2343 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_context/SearchControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_context/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      440 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_context/arg_buckets_utils.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.337390 argrelay-0.7.1.dev7/src/argrelay/runtime_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_data/AssignedValue.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      407 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_data/ClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_data/ConnectionConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      549 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_data/EnvelopeCollection.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      313 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_data/PluginEntry.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_data/ServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      455 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_data/ServerPluginControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      556 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_data/StaticData.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev7/src/argrelay/runtime_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.337390 argrelay-0.7.1.dev7/src/argrelay/sample_conf/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      207 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/src/argrelay/sample_conf/argrelay_client.json
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    35513 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/sample_conf/argrelay_server.yaml
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.337390 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2370 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_client/ClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1005 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_client/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.338390 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2839 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      736 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      976 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1767 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/MongoConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1068 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1054 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6371 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/ServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1822 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1148 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/StaticDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.339390 argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4775 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1968 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1544 2024-04-22 16:25:28.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      953 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/InitControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2943 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/SearchControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.339390 argrelay-0.7.1.dev7/src/argrelay/schema_config_plugin/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1465 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_plugin/PluginEntrySchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/schema_config_plugin/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.339390 argrelay-0.7.1.dev7/src/argrelay/schema_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2634 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/src/argrelay/schema_request/CallContextSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/schema_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.340390 argrelay-0.7.1.dev7/src/argrelay/schema_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      272 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/schema_response/ArgValues.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1221 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_response/ArgValuesSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_response/AssignedValueSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2763 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_response/EnvelopeContainerSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2433 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/schema_response/InterpResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2217 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_response/InterpResultSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1802 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/schema_response/InvocationInput.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev7/src/argrelay/schema_response/InvocationInputSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev7/src/argrelay/schema_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.341390 argrelay-0.7.1.dev7/src/argrelay/server_spec/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev7/src/argrelay/server_spec/CallContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/server_spec/DescribeLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1356 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/server_spec/ProposeArgValuesSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1410 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/server_spec/RelayLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.1.dev7/src/argrelay/server_spec/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      612 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev7/src/argrelay/server_spec/const_int.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3140 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/server_spec/server_data_schema.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.342390 argrelay-0.7.1.dev7/src/argrelay/test_infra/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      804 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/BaseTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2886 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/ClientServerTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1435 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/CustomTestCase.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2039 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/CustomVerifier.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7157 2024-05-19 16:07:53.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/End2EndTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    37764 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/EnvMockBuilder.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12616 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/InOutTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1425 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/JsonTestOutputVerifier.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1374 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/LocalClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2785 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/LocalClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4990 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/LocalTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      822 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/OpenFileMock.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3449 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/PopenMock.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4519 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/RemoteTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2353 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/ServerOnlyTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1375 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/TestCase.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2104 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev7/src/argrelay/test_infra/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 02:54:25.322390 argrelay-0.7.1.dev7/src/argrelay.egg-info/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-05-25 02:54:25.000000 argrelay-0.7.1.dev7/src/argrelay.egg-info/PKG-INFO
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31836 2024-05-25 02:54:25.000000 argrelay-0.7.1.dev7/src/argrelay.egg-info/SOURCES.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2024-05-25 02:54:25.000000 argrelay-0.7.1.dev7/src/argrelay.egg-info/dependency_links.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      195 2024-05-25 02:54:25.000000 argrelay-0.7.1.dev7/src/argrelay.egg-info/requires.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2024-05-25 02:54:25.000000 argrelay-0.7.1.dev7/src/argrelay.egg-info/top_level.txt
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.307904 argrelay-0.7.1.dev8/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2024-05-19 10:16:55.000000 argrelay-0.7.1.dev8/LICENSE
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-05-25 03:15:57.307904 argrelay-0.7.1.dev8/PKG-INFO
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.267904 argrelay-0.7.1.dev8/docs/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.269904 argrelay-0.7.1.dev8/docs/dev_notes/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5535 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/docs/dev_notes/bootstrap_procedure.1.project_creation.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2509 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1924 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/dev_notes/brief_history.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2781 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/dev_notes/code_style.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev8/docs/dev_notes/completion_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6986 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/dev_notes/completion_perf_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/dev_notes/gui_tests_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5196 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/dev_notes/how_search_works.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2495 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/dev_notes/library_vs_framework.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/dev_notes/mongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1469 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/docs/dev_notes/next_steps_tutorial.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3776 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/dev_notes/origin_story.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7809 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/dev_notes/query_perf_10_x_more_data_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7149 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/dev_notes/query_perf_cache_vs_no_cache.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4285 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/dev_notes/query_perf_mongomock_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8388 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/dev_notes/query_perf_pymongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev8/docs/dev_notes/release_procedure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      769 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/dev_notes/screencast_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      787 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/docs/dev_notes/scripts_summary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1128 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/docs/dev_notes/semver_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5697 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/docs/dev_notes/term_dictionary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11129 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/dev_notes/top_todos.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3241 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/dev_notes/version_format.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.274904 argrelay-0.7.1.dev8/docs/feature_stories/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3725 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_00_13_77_97.plugin_framework.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_01_89_09_24.interp_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      778 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2912 2024-04-21 14:23:13.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      228 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1839 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      994 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      770 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_14_59_14_06.pending_requests.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1130 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_15_79_76_85.line_processor.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1476 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1028 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      761 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_20_88_05_60.named_args.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1914 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      917 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_26_43_73_72.func_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_27_16_67_19.line_syntax.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3596 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_29_54_67_86.dir_structure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1029 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_31_70_49_15.search_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      649 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_33_76_82_84.composite_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1829 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_36_17_84_44.check_env.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1764 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      849 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_39_58_01_91.query_cache.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1739 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1450 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_43_50_57_71.echo_args_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      792 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_46_96_59_05.init_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1278 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_47_63_35_61.env_vars.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1348 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1556 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_55_57_45_04.enum_selector.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2481 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1744 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_58_61_77_69.dev_shell.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      751 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1457 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_62_25_92_06.assigned_context.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1211 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_63_63_14_08.generated_config.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4075 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_66_17_43_42.test_infra.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2246 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_67_16_61_97.git_plugin.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1507 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_71_87_33_52.help_hint.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1916 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_72_40_53_00.fill_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_72_53_55_13.show_non_default_options.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_74_69_61_79.get_set_data_envelope.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1370 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      155 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_78_91_27_22.interp_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_80_45_89_81.integrated_functions.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2391 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2089 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4514 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      493 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1841 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1735 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_91_88_07_23.jump_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3287 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_92_75_93_01.clean_command_line.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_94_30_49_28.help_doc.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1653 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_97_64_39_94.arg_buckets.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      189 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_98_55_40_77.invoke_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      505 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/feature_stories/FS_99_81_19_25.no_space_in_options.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      454 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/feature_stories/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      637 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.276904 argrelay-0.7.1.dev8/docs/release_notes/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1240 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      165 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.0.0.dev0.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1368 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.0.0.dev27.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.0.0.dev28.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      133 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.0.0.dev42.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.0.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       37 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.1.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       98 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.2.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       75 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.2.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      124 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.3.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      273 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.4.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      328 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.5.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      136 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.5.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      245 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.5.2.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      403 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.6.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      411 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.6.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      110 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.6.2.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       62 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.6.3.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      143 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/release_notes/v0.6.4.final.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.279904 argrelay-0.7.1.dev8/docs/task_refs/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      573 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      336 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_04_84_79_11.reorganize_tests_for_CI.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      277 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_11_77_28_50.suggestions_in_all_responses.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      418 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_24_22_11_49.avoid_removing_last_history_command.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2979 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_26_15_31_78.categorize_git_repo_existence.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_27_61_22_18.make_shell_vars_local.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2661 2024-05-25 03:08:09.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_30_69_19_14.infinite_spinner.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      459 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_32_99_70_35.JSONPath_to_verify_response_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_37_15_12_91.Popen_mock.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      352 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_40_10_18_32.add_custom_base_to_all_schemas.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      349 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_43_41_95_86.use_server_logger_to_disable_stdout.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      560 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       85 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      703 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      497 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_all_packages_before_test.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      640 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      224 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_70_48_96_29.be_able_to_assert_remaining_arg_vals.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      422 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_75_52_01_67.arg_buckets_to_support_multiple_var_args.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      170 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_79_67_28_83.recursive_dict_schema.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      187 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      456 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      652 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3051 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      256 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/docs/task_refs/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.280904 argrelay-0.7.1.dev8/docs/test_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      695 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev8/docs/test_data/TD_38_03_48_51.large_data_set.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      387 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11158 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/test_data/TD_63_37_05_36.demo_services_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.7.1.dev8/docs/test_data/TD_70_69_38_46.no_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      550 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev8/docs/test_data/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.7.1.dev8/pyproject.toml
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15739 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2024-05-25 03:15:57.307904 argrelay-0.7.1.dev8/setup.cfg
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4262 2024-05-25 03:08:09.000000 argrelay-0.7.1.dev8/setup.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.265905 argrelay-0.7.1.dev8/src/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.280904 argrelay-0.7.1.dev8/src/argrelay/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev8/src/argrelay/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.281904 argrelay-0.7.1.dev8/src/argrelay/client_command_local/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1714 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_local/AbstractLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      997 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_local/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.282904 argrelay-0.7.1.dev8/src/argrelay/client_command_remote/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2304 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      857 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3981 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/client_command_remote/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.282904 argrelay-0.7.1.dev8/src/argrelay/client_spec/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3787 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/src/argrelay/client_spec/ShellContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/client_spec/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.283904 argrelay-0.7.1.dev8/src/argrelay/composite_tree/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      344 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeForest.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1138 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeForestSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2071 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeInfoType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1144 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeNode.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6371 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeNodeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      657 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeNodeType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13703 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeTreeWalker.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11778 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/composite_tree/DictTreeWalker.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/composite_tree/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.285904 argrelay-0.7.1.dev8/src/argrelay/custom_integ/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8164 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/BaseConfigDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2325 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/ConfigOnlyDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3643 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3533 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/ConfigOnlyLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1598 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1737 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/FuncConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1492 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8075 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1869 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12644 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1615 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      853 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/ServiceArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    18325 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/ServiceDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      217 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/ServiceEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    69098 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/ServiceLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      842 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2512 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/git_utils.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      413 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ/value_constants.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.286904 argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7009 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/argrelay_common_lib.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    33035 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     7248 2024-05-19 16:53:10.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/check_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     3390 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/dev_shell.bash
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3713 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/init_shell_env.bash
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8092 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/shell_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     2908 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/upgrade_all_packages.bash
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.287904 argrelay-0.7.1.dev8/src/argrelay/enum_desc/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1313 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/ArgSource.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1011 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/CallConv.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1498 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/CompScope.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2952 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/CompType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4670 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/DistinctValuesQuery.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/InterpStep.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      470 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/PluginType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      547 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/ReservedArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      190 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/ReservedEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1707 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/RunMode.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/ServerAction.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      390 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/SpecialChar.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      511 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/SpecialFunc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3091 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/TermColor.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1259 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/TokenType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev8/src/argrelay/enum_desc/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.288904 argrelay-0.7.1.dev8/src/argrelay/handler_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/src/argrelay/handler_request/AbstractServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      986 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3103 2024-04-22 16:25:28.000000 argrelay-0.7.1.dev8/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/handler_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.289904 argrelay-0.7.1.dev8/src/argrelay/handler_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      200 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/handler_response/AbstractClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9401 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1122 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1023 2024-04-13 16:33:00.000000 argrelay-0.7.1.dev8/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/handler_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.289904 argrelay-0.7.1.dev8/src/argrelay/misc_helper_common/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-05-18 02:28:39.000000 argrelay-0.7.1.dev8/src/argrelay/misc_helper_common/ElapsedTime.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      741 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/misc_helper_common/ObjectSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/misc_helper_common/TypeDesc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/src/argrelay/misc_helper_common/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.289904 argrelay-0.7.1.dev8/src/argrelay/misc_helper_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      521 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/misc_helper_server/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.290904 argrelay-0.7.1.dev8/src/argrelay/mongo_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev8/src/argrelay/mongo_data/MongoClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3649 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/mongo_data/MongoClientWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      616 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/mongo_data/MongoConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/mongo_data/MongoServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2086 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/mongo_data/MongoServerWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.1.dev8/src/argrelay/mongo_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.290904 argrelay-0.7.1.dev8/src/argrelay/plugin_config/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4367 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_config/AbstractConfigurator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4265 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_config/DefaultConfigurator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_config/DefaultConfiguratorConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1555 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_config/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.291904 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5958 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/AbstractDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4218 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/AbstractJumpDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1697 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/AbstractJumpDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2087 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/EchoDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1516 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/ErrorDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5791 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/HelpDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5308 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/InterceptDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      870 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/NoopDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1813 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/QueryEnumDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-08-06 08:09:50.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.293904 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3681 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/AbstractInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2278 2024-04-22 16:25:28.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/AbstractInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      701 2024-05-23 10:51:14.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FirstArgInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5508 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FirstArgInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1349 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    17429 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FuncTreeInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12865 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FuncTreeInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1684 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7238 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/InterpTreeInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6270 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/InterpTreeInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2925 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      384 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/NoopInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/NoopInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.293904 argrelay-0.7.1.dev8/src/argrelay/plugin_loader/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_loader/AbstractLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-12-14 14:18:48.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_loader/NoopLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/plugin_loader/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.294904 argrelay-0.7.1.dev8/src/argrelay/relay_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      965 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/relay_client/AbstractClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      366 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/relay_client/AbstractClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      266 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/relay_client/AbstractClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-10-21 04:19:27.000000 argrelay-0.7.1.dev8/src/argrelay/relay_client/RemoteClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1861 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/relay_client/RemoteClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.7.1.dev8/src/argrelay/relay_client/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2821 2024-05-25 03:08:09.000000 argrelay-0.7.1.dev8/src/argrelay/relay_client/__main__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4197 2024-05-25 03:08:29.000000 argrelay-0.7.1.dev8/src/argrelay/relay_client/proc_spinner.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2733 2024-05-25 03:08:09.000000 argrelay-0.7.1.dev8/src/argrelay/relay_client/proc_split.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2926 2024-05-25 03:08:09.000000 argrelay-0.7.1.dev8/src/argrelay/relay_client/proc_worker.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.295904 argrelay-0.7.1.dev8/src/argrelay/relay_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11191 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/CustomFlaskApp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/GuiBannerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1500 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/HelpHintCache.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7312 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/LocalServer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/QueryCacheConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13331 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/QueryEngine.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1147 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/QueryResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/__main__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.296904 argrelay-0.7.1.dev8/src/argrelay/relay_server/gui_static/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31127 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/gui_static/argrelay_client.js
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      318 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/gui_static/argrelay_favicon.ico
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4987 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/gui_static/argrelay_style.css
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/gui_static/external_link.svg
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.296904 argrelay-0.7.1.dev8/src/argrelay/relay_server/gui_templates/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7812 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/gui_templates/argrelay_main.html
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4947 2024-05-17 16:12:06.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/route_api.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1894 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/relay_server/route_gui.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.297904 argrelay-0.7.1.dev8/src/argrelay/runtime_context/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3180 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_context/AbstractPlugin.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4398 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_context/EnvelopeContainer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_context/InitControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    17397 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_context/InterpContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6354 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_context/ParsedContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2343 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_context/SearchControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_context/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      440 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_context/arg_buckets_utils.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.298904 argrelay-0.7.1.dev8/src/argrelay/runtime_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_data/AssignedValue.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      407 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_data/ClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_data/ConnectionConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      549 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_data/EnvelopeCollection.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      313 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_data/PluginEntry.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_data/ServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      455 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_data/ServerPluginControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      556 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_data/StaticData.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev8/src/argrelay/runtime_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.298904 argrelay-0.7.1.dev8/src/argrelay/sample_conf/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      207 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/src/argrelay/sample_conf/argrelay_client.json
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    35513 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/sample_conf/argrelay_server.yaml
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.298904 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2370 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_client/ClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1005 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_client/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.299904 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2839 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      736 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      976 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1767 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/MongoConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1068 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1054 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6371 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/ServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1822 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1148 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/StaticDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.300904 argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4775 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1968 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1544 2024-04-22 16:25:28.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      953 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/InitControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2943 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/SearchControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.300904 argrelay-0.7.1.dev8/src/argrelay/schema_config_plugin/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1465 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_plugin/PluginEntrySchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/schema_config_plugin/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.300904 argrelay-0.7.1.dev8/src/argrelay/schema_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2634 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/src/argrelay/schema_request/CallContextSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/schema_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.301904 argrelay-0.7.1.dev8/src/argrelay/schema_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      272 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/schema_response/ArgValues.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1221 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_response/ArgValuesSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_response/AssignedValueSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2763 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_response/EnvelopeContainerSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2433 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/schema_response/InterpResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2217 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_response/InterpResultSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1802 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/schema_response/InvocationInput.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev8/src/argrelay/schema_response/InvocationInputSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev8/src/argrelay/schema_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.301904 argrelay-0.7.1.dev8/src/argrelay/server_spec/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev8/src/argrelay/server_spec/CallContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/server_spec/DescribeLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1356 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/server_spec/ProposeArgValuesSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1410 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/server_spec/RelayLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.1.dev8/src/argrelay/server_spec/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      612 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev8/src/argrelay/server_spec/const_int.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3140 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/server_spec/server_data_schema.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.303904 argrelay-0.7.1.dev8/src/argrelay/test_infra/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      804 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/BaseTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2886 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/ClientServerTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1435 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/CustomTestCase.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2039 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/CustomVerifier.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7157 2024-05-19 16:07:53.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/End2EndTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    37764 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/EnvMockBuilder.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12616 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/InOutTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1425 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/JsonTestOutputVerifier.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1374 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/LocalClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2785 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/LocalClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4990 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/LocalTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      822 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/OpenFileMock.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3449 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/PopenMock.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4519 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/RemoteTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2353 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/ServerOnlyTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1375 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/TestCase.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2104 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev8/src/argrelay/test_infra/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 03:15:57.280904 argrelay-0.7.1.dev8/src/argrelay.egg-info/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-05-25 03:15:57.000000 argrelay-0.7.1.dev8/src/argrelay.egg-info/PKG-INFO
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31836 2024-05-25 03:15:57.000000 argrelay-0.7.1.dev8/src/argrelay.egg-info/SOURCES.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2024-05-25 03:15:57.000000 argrelay-0.7.1.dev8/src/argrelay.egg-info/dependency_links.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      195 2024-05-25 03:15:57.000000 argrelay-0.7.1.dev8/src/argrelay.egg-info/requires.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2024-05-25 03:15:57.000000 argrelay-0.7.1.dev8/src/argrelay.egg-info/top_level.txt
```

### Comparing `argrelay-0.7.1.dev7/LICENSE` & `argrelay-0.7.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/PKG-INFO` & `argrelay-0.7.1.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.7.1.dev7
+Version: 0.7.1.dev8
 Summary: Tab-completion & data search server = total recall for Bash shell
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/bootstrap_procedure.1.project_creation.md` & `argrelay-0.7.1.dev8/docs/dev_notes/bootstrap_procedure.1.project_creation.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md` & `argrelay-0.7.1.dev8/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md` & `argrelay-0.7.1.dev8/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/brief_history.md` & `argrelay-0.7.1.dev8/docs/dev_notes/brief_history.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/code_style.md` & `argrelay-0.7.1.dev8/docs/dev_notes/code_style.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/completion_notes.md` & `argrelay-0.7.1.dev8/docs/dev_notes/completion_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/completion_perf_notes.md` & `argrelay-0.7.1.dev8/docs/dev_notes/completion_perf_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/gui_tests_notes.md` & `argrelay-0.7.1.dev8/docs/dev_notes/gui_tests_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/how_search_works.md` & `argrelay-0.7.1.dev8/docs/dev_notes/how_search_works.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/library_vs_framework.md` & `argrelay-0.7.1.dev8/docs/dev_notes/library_vs_framework.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/mongo_notes.md` & `argrelay-0.7.1.dev8/docs/dev_notes/mongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/next_steps_tutorial.md` & `argrelay-0.7.1.dev8/docs/dev_notes/next_steps_tutorial.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/origin_story.md` & `argrelay-0.7.1.dev8/docs/dev_notes/origin_story.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/query_perf_10_x_more_data_notes.md` & `argrelay-0.7.1.dev8/docs/dev_notes/query_perf_10_x_more_data_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/query_perf_cache_vs_no_cache.md` & `argrelay-0.7.1.dev8/docs/dev_notes/query_perf_cache_vs_no_cache.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/query_perf_mongomock_notes.md` & `argrelay-0.7.1.dev8/docs/dev_notes/query_perf_mongomock_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/query_perf_pymongo_notes.md` & `argrelay-0.7.1.dev8/docs/dev_notes/query_perf_pymongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/release_procedure.md` & `argrelay-0.7.1.dev8/docs/dev_notes/release_procedure.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/screencast_notes.md` & `argrelay-0.7.1.dev8/docs/dev_notes/screencast_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/scripts_summary.md` & `argrelay-0.7.1.dev8/docs/dev_notes/scripts_summary.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/semver_notes.md` & `argrelay-0.7.1.dev8/docs/dev_notes/semver_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/term_dictionary.md` & `argrelay-0.7.1.dev8/docs/dev_notes/term_dictionary.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/top_todos.md` & `argrelay-0.7.1.dev8/docs/dev_notes/top_todos.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/dev_notes/version_format.md` & `argrelay-0.7.1.dev8/docs/dev_notes/version_format.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_00_13_77_97.plugin_framework.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_00_13_77_97.plugin_framework.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_01_89_09_24.interp_tree.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_01_89_09_24.interp_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_06_99_43_60.list_arg_value.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_06_99_43_60.list_arg_value.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_14_59_14_06.pending_requests.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_14_59_14_06.pending_requests.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_15_79_76_85.line_processor.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_15_79_76_85.line_processor.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_20_88_05_60.named_args.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_20_88_05_60.named_args.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_26_43_73_72.func_tree.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_26_43_73_72.func_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_27_16_67_19.line_syntax.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_27_16_67_19.line_syntax.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_29_54_67_86.dir_structure.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_29_54_67_86.dir_structure.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_31_70_49_15.search_control.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_31_70_49_15.search_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_33_76_82_84.composite_tree.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_33_76_82_84.composite_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_36_17_84_44.check_env.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_36_17_84_44.check_env.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_39_58_01_91.query_cache.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_39_58_01_91.query_cache.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_47_63_35_61.env_vars.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_47_63_35_61.env_vars.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_55_57_45_04.enum_selector.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_55_57_45_04.enum_selector.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_58_61_77_69.dev_shell.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_58_61_77_69.dev_shell.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_62_25_92_06.assigned_context.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_62_25_92_06.assigned_context.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_63_63_14_08.generated_config.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_63_63_14_08.generated_config.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_66_17_43_42.test_infra.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_66_17_43_42.test_infra.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_67_16_61_97.git_plugin.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_67_16_61_97.git_plugin.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_71_87_33_52.help_hint.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_71_87_33_52.help_hint.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_72_40_53_00.fill_control.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_72_40_53_00.fill_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_80_45_89_81.integrated_functions.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_80_45_89_81.integrated_functions.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_91_88_07_23.jump_tree.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_91_88_07_23.jump_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_92_75_93_01.clean_command_line.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_92_75_93_01.clean_command_line.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/feature_stories/FS_97_64_39_94.arg_buckets.md` & `argrelay-0.7.1.dev8/docs/feature_stories/FS_97_64_39_94.arg_buckets.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/readme.md` & `argrelay-0.7.1.dev8/docs/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/release_notes/readme.md` & `argrelay-0.7.1.dev8/docs/release_notes/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/release_notes/v0.0.0.dev27.md` & `argrelay-0.7.1.dev8/docs/release_notes/v0.0.0.dev27.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md` & `argrelay-0.7.1.dev8/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md` & `argrelay-0.7.1.dev8/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md` & `argrelay-0.7.1.dev8/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/task_refs/TODO_30_69_19_14.infinite_spinner.md` & `argrelay-0.7.1.dev8/docs/task_refs/TODO_30_69_19_14.infinite_spinner.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md` & `argrelay-0.7.1.dev8/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md` & `argrelay-0.7.1.dev8/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md` & `argrelay-0.7.1.dev8/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md` & `argrelay-0.7.1.dev8/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md` & `argrelay-0.7.1.dev8/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md` & `argrelay-0.7.1.dev8/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/test_data/TD_63_37_05_36.demo_services_data.md` & `argrelay-0.7.1.dev8/docs/test_data/TD_63_37_05_36.demo_services_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/test_data/TD_70_69_38_46.no_data.md` & `argrelay-0.7.1.dev8/docs/test_data/TD_70_69_38_46.no_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md` & `argrelay-0.7.1.dev8/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md` & `argrelay-0.7.1.dev8/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/readme.md` & `argrelay-0.7.1.dev8/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/setup.py` & `argrelay-0.7.1.dev8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # All paths start with `top_dir_path`:
     return file_paths
 
 
 setuptools.setup(
     name = "argrelay",
     # See `docs/dev_notes/version_format.md`:
-    version = "0.7.1.dev7",
+    version = "0.7.1.dev8",
     author = "uvsmtid",
     author_email = "uvsmtid@gmail.com",
     description = "Tab-completion & data search server = total recall for Bash shell",
     long_description = """
 See: https://github.com/argrelay/argrelay
     """,
     long_description_content_type = "text/markdown",
```

### Comparing `argrelay-0.7.1.dev7/src/argrelay/client_command_local/AbstractLocalClientCommand.py` & `argrelay-0.7.1.dev8/src/argrelay/client_command_local/AbstractLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py` & `argrelay-0.7.1.dev8/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py` & `argrelay-0.7.1.dev8/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py` & `argrelay-0.7.1.dev8/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py` & `argrelay-0.7.1.dev8/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py` & `argrelay-0.7.1.dev8/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py` & `argrelay-0.7.1.dev8/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py` & `argrelay-0.7.1.dev8/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py` & `argrelay-0.7.1.dev8/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/client_spec/ShellContext.py` & `argrelay-0.7.1.dev8/src/argrelay/client_spec/ShellContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeForestSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeForestSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeInfoType.py` & `argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeInfoType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeNode.py` & `argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeNode.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeNodeSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeNodeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeNodeType.py` & `argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeNodeType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/composite_tree/CompositeTreeWalker.py` & `argrelay-0.7.1.dev8/src/argrelay/composite_tree/CompositeTreeWalker.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/composite_tree/DictTreeWalker.py` & `argrelay-0.7.1.dev8/src/argrelay/composite_tree/DictTreeWalker.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/BaseConfigDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/BaseConfigDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/ConfigOnlyDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/ConfigOnlyDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/ConfigOnlyLoader.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/ConfigOnlyLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/FuncConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/FuncConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoArgType.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoLoader.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/ServiceArgType.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/ServiceArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/ServiceDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/ServiceDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/ServiceLoader.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/ServiceLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ/git_utils.py` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ/git_utils.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/argrelay_common_lib.bash` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/argrelay_common_lib.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/bootstrap_dev_env.bash` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/bootstrap_dev_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/check_env.bash` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/check_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/dev_shell.bash` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/dev_shell.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/init_shell_env.bash` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/init_shell_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/shell_env.bash` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/shell_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/custom_integ_res/upgrade_all_packages.bash` & `argrelay-0.7.1.dev8/src/argrelay/custom_integ_res/upgrade_all_packages.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/enum_desc/ArgSource.py` & `argrelay-0.7.1.dev8/src/argrelay/enum_desc/ArgSource.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/enum_desc/CallConv.py` & `argrelay-0.7.1.dev8/src/argrelay/enum_desc/CallConv.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/enum_desc/CompScope.py` & `argrelay-0.7.1.dev8/src/argrelay/enum_desc/CompScope.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/enum_desc/CompType.py` & `argrelay-0.7.1.dev8/src/argrelay/enum_desc/CompType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/enum_desc/DistinctValuesQuery.py` & `argrelay-0.7.1.dev8/src/argrelay/enum_desc/DistinctValuesQuery.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/enum_desc/ReservedArgType.py` & `argrelay-0.7.1.dev8/src/argrelay/enum_desc/ReservedArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/enum_desc/RunMode.py` & `argrelay-0.7.1.dev8/src/argrelay/enum_desc/RunMode.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/enum_desc/TermColor.py` & `argrelay-0.7.1.dev8/src/argrelay/enum_desc/TermColor.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/enum_desc/TokenType.py` & `argrelay-0.7.1.dev8/src/argrelay/enum_desc/TokenType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/handler_request/AbstractServerRequestHandler.py` & `argrelay-0.7.1.dev8/src/argrelay/handler_request/AbstractServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py` & `argrelay-0.7.1.dev8/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py` & `argrelay-0.7.1.dev8/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py` & `argrelay-0.7.1.dev8/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py` & `argrelay-0.7.1.dev8/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py` & `argrelay-0.7.1.dev8/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py` & `argrelay-0.7.1.dev8/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/misc_helper_common/ElapsedTime.py` & `argrelay-0.7.1.dev8/src/argrelay/misc_helper_common/ElapsedTime.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/misc_helper_common/ObjectSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/misc_helper_common/ObjectSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/misc_helper_common/TypeDesc.py` & `argrelay-0.7.1.dev8/src/argrelay/misc_helper_common/TypeDesc.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/misc_helper_common/__init__.py` & `argrelay-0.7.1.dev8/src/argrelay/misc_helper_common/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/misc_helper_server/__init__.py` & `argrelay-0.7.1.dev8/src/argrelay/misc_helper_server/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/mongo_data/MongoClientWrapper.py` & `argrelay-0.7.1.dev8/src/argrelay/mongo_data/MongoClientWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/mongo_data/MongoConfig.py` & `argrelay-0.7.1.dev8/src/argrelay/mongo_data/MongoConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/mongo_data/MongoServerWrapper.py` & `argrelay-0.7.1.dev8/src/argrelay/mongo_data/MongoServerWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_config/AbstractConfigurator.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_config/AbstractConfigurator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_config/DefaultConfigurator.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_config/DefaultConfigurator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_config/DefaultConfiguratorConfig.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_config/DefaultConfiguratorConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/AbstractDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/AbstractDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/AbstractJumpDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/AbstractJumpDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/AbstractJumpDelegatorConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/AbstractJumpDelegatorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/EchoDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/EchoDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/ErrorDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/ErrorDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/HelpDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/HelpDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/InterceptDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/InterceptDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/NoopDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/NoopDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_delegator/QueryEnumDelegator.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_delegator/QueryEnumDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/AbstractInterp.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/AbstractInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/AbstractInterpFactory.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/AbstractInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FirstArgInterp.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FirstArgInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FirstArgInterpFactory.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FirstArgInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FuncTreeInterp.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FuncTreeInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FuncTreeInterpFactory.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FuncTreeInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/InterpTreeInterp.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/InterpTreeInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/InterpTreeInterpFactory.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/InterpTreeInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/plugin_interp/NoopInterpFactory.py` & `argrelay-0.7.1.dev8/src/argrelay/plugin_interp/NoopInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_client/AbstractClient.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_client/AbstractClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_client/RemoteClient.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_client/RemoteClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_client/RemoteClientCommandFactory.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_client/RemoteClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_client/__main__.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_client/__main__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_client/proc_spinner.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_client/proc_spinner.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -75,18 +75,18 @@
     child_pid: int,
 ):
     (
         child_pid,
         child_status,
     ) = os.waitpid(child_pid, os.WNOHANG)
     if child_pid == 0 and child_status == 0:
-        assert has_child_exited
+        assert not has_child_exited
         return True
     else:
-        assert not has_child_exited
+        assert has_child_exited
         return False
 
 
 def generate_pending_cursor():
     cursor_states = [
         f"{TermColor.spinner_color.value}/|\\|{TermColor.reset_style.value}",
         f"{TermColor.spinner_color.value}|/|\\{TermColor.reset_style.value}",
```

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_client/proc_split.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_client/proc_split.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_client/proc_worker.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_client/proc_worker.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_server/CustomFlaskApp.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_server/CustomFlaskApp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_server/HelpHintCache.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_server/HelpHintCache.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_server/LocalServer.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_server/LocalServer.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_server/QueryEngine.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_server/QueryEngine.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_server/QueryResult.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_server/QueryResult.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_server/gui_static/argrelay_client.js` & `argrelay-0.7.1.dev8/src/argrelay/relay_server/gui_static/argrelay_client.js`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_server/gui_static/argrelay_style.css` & `argrelay-0.7.1.dev8/src/argrelay/relay_server/gui_static/argrelay_style.css`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_server/gui_templates/argrelay_main.html` & `argrelay-0.7.1.dev8/src/argrelay/relay_server/gui_templates/argrelay_main.html`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_server/route_api.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_server/route_api.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/relay_server/route_gui.py` & `argrelay-0.7.1.dev8/src/argrelay/relay_server/route_gui.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/runtime_context/AbstractPlugin.py` & `argrelay-0.7.1.dev8/src/argrelay/runtime_context/AbstractPlugin.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/runtime_context/EnvelopeContainer.py` & `argrelay-0.7.1.dev8/src/argrelay/runtime_context/EnvelopeContainer.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/runtime_context/InterpContext.py` & `argrelay-0.7.1.dev8/src/argrelay/runtime_context/InterpContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/runtime_context/ParsedContext.py` & `argrelay-0.7.1.dev8/src/argrelay/runtime_context/ParsedContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/runtime_context/SearchControl.py` & `argrelay-0.7.1.dev8/src/argrelay/runtime_context/SearchControl.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/runtime_data/EnvelopeCollection.py` & `argrelay-0.7.1.dev8/src/argrelay/runtime_data/EnvelopeCollection.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/runtime_data/ServerConfig.py` & `argrelay-0.7.1.dev8/src/argrelay/runtime_data/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/runtime_data/StaticData.py` & `argrelay-0.7.1.dev8/src/argrelay/runtime_data/StaticData.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/sample_conf/argrelay_server.yaml` & `argrelay-0.7.1.dev8/src/argrelay/sample_conf/argrelay_server.yaml`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_client/ClientConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_client/ClientConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/MongoConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/MongoConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/ServerConfigSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/ServerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_core_server/StaticDataSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_core_server/StaticDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/DataEnvelopeSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/DataEnvelopeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/InitControlSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/InitControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_interp/SearchControlSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_interp/SearchControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_config_plugin/PluginEntrySchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_config_plugin/PluginEntrySchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_request/CallContextSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_request/CallContextSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_response/ArgValuesSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_response/ArgValuesSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_response/AssignedValueSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_response/AssignedValueSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_response/EnvelopeContainerSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_response/EnvelopeContainerSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_response/InterpResult.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_response/InterpResult.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_response/InterpResultSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_response/InterpResultSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_response/InvocationInput.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_response/InvocationInput.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/schema_response/InvocationInputSchema.py` & `argrelay-0.7.1.dev8/src/argrelay/schema_response/InvocationInputSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/server_spec/CallContext.py` & `argrelay-0.7.1.dev8/src/argrelay/server_spec/CallContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/server_spec/DescribeLineArgsSpec.py` & `argrelay-0.7.1.dev8/src/argrelay/server_spec/DescribeLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/server_spec/ProposeArgValuesSpec.py` & `argrelay-0.7.1.dev8/src/argrelay/server_spec/ProposeArgValuesSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/server_spec/RelayLineArgsSpec.py` & `argrelay-0.7.1.dev8/src/argrelay/server_spec/RelayLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/server_spec/const_int.py` & `argrelay-0.7.1.dev8/src/argrelay/server_spec/const_int.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/server_spec/server_data_schema.py` & `argrelay-0.7.1.dev8/src/argrelay/server_spec/server_data_schema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/BaseTestClass.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/BaseTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/ClientServerTestClass.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/ClientServerTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/CustomTestCase.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/CustomTestCase.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/CustomVerifier.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/CustomVerifier.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/End2EndTestClass.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/End2EndTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/EnvMockBuilder.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/EnvMockBuilder.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/InOutTestClass.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/InOutTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/JsonTestOutputVerifier.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/JsonTestOutputVerifier.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/LocalClient.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/LocalClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/LocalClientCommandFactory.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/LocalClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/LocalTestClass.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/LocalTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/OpenFileMock.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/OpenFileMock.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/PopenMock.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/PopenMock.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/RemoteTestClass.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/RemoteTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/ServerOnlyTestClass.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/ServerOnlyTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/TestCase.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/TestCase.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay/test_infra/__init__.py` & `argrelay-0.7.1.dev8/src/argrelay/test_infra/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev7/src/argrelay.egg-info/PKG-INFO` & `argrelay-0.7.1.dev8/src/argrelay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.7.1.dev7
+Version: 0.7.1.dev8
 Summary: Tab-completion & data search server = total recall for Bash shell
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `argrelay-0.7.1.dev7/src/argrelay.egg-info/SOURCES.txt` & `argrelay-0.7.1.dev8/src/argrelay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

