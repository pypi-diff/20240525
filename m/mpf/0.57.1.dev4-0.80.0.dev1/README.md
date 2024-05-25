# Comparing `tmp/mpf-0.57.1.dev4.tar.gz` & `tmp/mpf-0.80.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpf-0.57.1.dev4.tar", last modified: Mon Apr 22 22:07:05 2024, max compression
+gzip compressed data, was "mpf-0.80.0.dev1.tar", last modified: Sat May 25 20:45:59 2024, max compression
```

## Comparing `mpf-0.57.1.dev4.tar` & `mpf-0.80.0.dev1.tar`

### file list

```diff
@@ -1,1661 +1,1665 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.397873 mpf-0.57.1.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/.bandit
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.229871 mpf-0.57.1.dev4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.229871 mpf-0.57.1.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/.github/workflows/build_wheels.yml
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/.github/workflows/prospector.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-22 22:07:05.397873 mpf-0.57.1.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.229871 mpf-0.57.1.dev4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.229871 mpf-0.57.1.dev4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.229871 mpf-0.57.1.dev4/docs/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.233871 mpf-0.57.1.dev4/docs/_static/images/icons/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9820 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-114x114.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     7640 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-120x120.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    11750 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-144x144.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    15171 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-152x152.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     3769 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-57x57.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     3533 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-60x60.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     5111 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-72x72.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     5829 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-76x76.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     8488 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/favicon-128.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      637 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/favicon-16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    23562 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/favicon-196x196.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1620 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/favicon-32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6167 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/favicon-96x96.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    34494 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/favicon.ico
--rwxr-xr-x   0 runner    (1001) docker     (127)    11750 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/mstile-144x144.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    30530 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/mstile-150x150.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    95427 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/mstile-310x150.png
--rwxr-xr-x   0 runner    (1001) docker     (127)   145659 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/mstile-310x310.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     8488 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/icons/mstile-70x70.png
--rw-r--r--   0 runner    (1001) docker     (127)    20225 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/mpf-logo-200.png
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/mpf-logo-tiny.png
--rw-r--r--   0 runner    (1001) docker     (127)   280785 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/images/mpf-logo-tiny@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_static/mpf.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.237871 mpf-0.57.1.dev4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/config_players.rst
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/config_players_overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/devices_overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/machine.rst
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/machine_overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/misc_overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/modes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/modes_overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/platforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/platforms_overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/self.machine.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/_templates/tests_overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.241871 mpf-0.57.1.dev4/docs/bcp/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/ball_end.rst
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/ball_start.rst
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/device.rst
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/error.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/goodbye.rst
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/hello.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/machine_variable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/mode_start.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/mode_stop.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/monitor_start.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/monitor_stop.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/player_added.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/player_turn_start.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/player_variable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/register_trigger.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/remove_trigger.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/reset.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/reset_complete.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/switch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/bcp/trigger.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.241871 mpf-0.57.1.dev4/docs/code/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/code/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/code/machine_code.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/code/mode_code.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18834 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.245871 mpf-0.57.1.dev4/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/dev/Send variables via self.machine.events.post.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/dev/dev_environment.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/dev/event_annotations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/dev/hardware.rst
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/dev/mc.widget_player.rst
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/dev/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.245871 mpf-0.57.1.dev4/docs/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/functions/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/functions/machine_variables.rst
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/functions/player_variables.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.245871 mpf-0.57.1.dev4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/images/custom_mode_code.png
--rw-r--r--   0 runner    (1001) docker     (127)    14947 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/images/scriptlet.png
--rw-r--r--   0 runner    (1001) docker     (127)    81139 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/images/test_classes.png
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.245871 mpf-0.57.1.dev4/docs/overview/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/overview/boot_process.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/overview/files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/overview/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/overview/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/overview/yaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.245871 mpf-0.57.1.dev4/docs/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/testing/fuzz_testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/testing/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/testing/running_mpf_tests.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.245871 mpf-0.57.1.dev4/docs/testing/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/testing/tutorial/1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/testing/tutorial/2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/testing/writing_machine_tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/docs/testing/writing_mpf_tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/get_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.249871 mpf-0.57.1.dev4/mpf/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.249871 mpf-0.57.1.dev4/mpf/assets/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31019 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/assets/show.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.249871 mpf-0.57.1.dev4/mpf/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.169870 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.169870 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.249871 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/events/config/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/events/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.169870 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/shows/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.249871 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/shows/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/shows/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.249871 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/shows/shows/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/shows/shows/minimal_light_show.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/shows/shows/minimal_light_show_token.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/shows/shows/multi_step_tags.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/shows/shows/single_step_tag.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.169870 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/switch_hits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.249871 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/switch_hits/config/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/machine_files/switch_hits/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/test_benchmark_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/test_benchmark_light_shows.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/benchmarks/test_benchmark_switch_hits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.253872 mpf-0.57.1.dev4/mpf/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/both.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/create_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/game.py
--rw-r--r--   0 runner    (1001) docker     (127)     9472 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/logging_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/commands/wire.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.257871 mpf-0.57.1.dev4/mpf/config_players/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/bcp_plugin_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/blinkenlight_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/block_event_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/coil_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/device_config_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/event_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/flasher_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/flat_config_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/hardware_sound_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/light_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/plugin_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/queue_event_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/queue_relay_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/random_event_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/score_queue_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/segment_display_player.py
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/show_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_players/variable_player.py
--rw-r--r--   0 runner    (1001) docker     (127)    87103 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/config_spec.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.265872 mpf-0.57.1.dev4/mpf/core/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40488 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/async_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/ball_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/ball_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.265872 mpf-0.57.1.dev4/mpf/core/bcp/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/bcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/bcp/bcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/bcp/bcp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35921 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/bcp/bcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/bcp/bcp_pickle_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/bcp/bcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/bcp/bcp_socket_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/bcp/bcp_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/case_insensitive_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)    13080 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16343 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/config_player.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10830 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/config_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/config_spec_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    28850 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/crash_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/custom_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/delays.py
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/device_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/enable_disable_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    40793 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/file_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/light_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    39389 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/machine_vars.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23375 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/mode_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/mode_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/mpf_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/placeholder_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/platform_batch_light_system.py
--rw-r--r--   0 runner    (1001) docker     (127)    23725 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/platform_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/randomizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21671 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/rgb_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/rgba_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    66242 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/segment_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/service_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/settings_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/show_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    30374 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/switch_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/system_wide_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    18930 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/text_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    30290 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/core/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.273872 mpf-0.57.1.dev4/mpf/devices/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/accelerometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/achievement.py
--rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/achievement_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/autofire.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.273872 mpf-0.57.1.dev4/mpf/devices/ball_device/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/ball_count_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    28823 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/ball_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/ball_device_ejector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/ball_device_state_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/default_ball_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/enable_coil_ejector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/entrance_switch_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/event_ejector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/hold_coil_ejector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/incoming_balls_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    27532 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/outgoing_balls_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/physical_ball_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/pulse_coil_ejector.py
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_device/switch_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_hold.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/ball_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/blinkenlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/combo_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/device_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/digital_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/digital_score_reel.py
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/diverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/dmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    18753 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    19396 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/drop_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/dual_wound_coil.py
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/extra_ball.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/extra_ball_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/flipper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/hardware_sound_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/kickback.py
--rw-r--r--   0 runner    (1001) docker     (127)    36761 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/light_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    23267 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/logic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/magnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/multiball.py
--rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/multiball_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    16670 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/playfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/playfield_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/power_supply_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/rgb_dmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/score_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/score_reel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/score_reel_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/score_reel_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.273872 mpf-0.57.1.dev4/mpf/devices/segment_display/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/segment_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18898 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/segment_display/segment_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/segment_display/segment_display_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/segment_display/text_stack_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/segment_display/transition_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    22277 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/segment_display/transitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/sequence_shot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/servo.py
--rw-r--r--   0 runner    (1001) docker     (127)    19220 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/shot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/shot_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/shot_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/show_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/speedometer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/stepper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/timed_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    21260 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/devices/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.273872 mpf-0.57.1.dev4/mpf/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/exceptions/base_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/exceptions/config_file_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/exceptions/driver_limits_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/exceptions/runtime_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/file_interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/file_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/file_interfaces/pickle_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/file_interfaces/yaml_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/attract/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/attract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/attract/code/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/attract/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/attract/code/attract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/attract/config/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/attract/config/attract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/bonus/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/bonus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/bonus/code/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/bonus/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/bonus/code/bonus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/bonus/config/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/bonus/config/bonus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/carousel/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/carousel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/carousel/code/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/carousel/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/carousel/code/carousel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/credits/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/credits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/credits/code/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/credits/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27935 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/credits/code/credits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/credits/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/credits/config/credits.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/game/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/game/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/game/code/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/game/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31533 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/game/code/game.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/game/config/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/game/config/game.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/high_score/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/high_score/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/high_score/code/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/high_score/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/high_score/code/high_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/high_score/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/high_score/config/high_score.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/high_score/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/high_score/images/back_arrow_7x7.png
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/high_score/images/back_arrow_7x7_selected.png
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/high_score/images/end_11x7.png
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/high_score/images/end_11x7_selected.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.173870 mpf-0.57.1.dev4/mpf/modes/match/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/match/code/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/match/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/match/code/match.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.277872 mpf-0.57.1.dev4/mpf/modes/match/config/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/match/config/match.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.281872 mpf-0.57.1.dev4/mpf/modes/service/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.281872 mpf-0.57.1.dev4/mpf/modes/service/code/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34256 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/service/code/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.281872 mpf-0.57.1.dev4/mpf/modes/service/config/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/service/config/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.281872 mpf-0.57.1.dev4/mpf/modes/service/sounds/
--rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/service/sounds/power_off.ogg
--rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/service/sounds/switch_hit.ogg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.173870 mpf-0.57.1.dev4/mpf/modes/service_dmd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.281872 mpf-0.57.1.dev4/mpf/modes/service_dmd/config/
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/service_dmd/config/service_dmd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.173870 mpf-0.57.1.dev4/mpf/modes/service_segment_display/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.281872 mpf-0.57.1.dev4/mpf/modes/service_segment_display/config/
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/service_segment_display/config/service_segment_display.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.281872 mpf-0.57.1.dev4/mpf/modes/tilt/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/tilt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.281872 mpf-0.57.1.dev4/mpf/modes/tilt/code/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/tilt/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/tilt/code/tilt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.281872 mpf-0.57.1.dev4/mpf/modes/tilt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/modes/tilt/config/tilt.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/mpfconfig.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.281872 mpf-0.57.1.dev4/mpf/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/parsers/event_reference_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/parsers/special_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.285872 mpf-0.57.1.dev4/mpf/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/base_serial_communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/driver_light_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fadecandy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.285872 mpf-0.57.1.dev4/mpf/platforms/fast/
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/TODO.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.289872 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/aud.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/dmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/emu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/net_nano.py
--rw-r--r--   0 runner    (1001) docker     (127)    13610 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/net_neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/net_retro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/rgb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/communicators/seg.py
--rw-r--r--   0 runner    (1001) docker     (127)    38995 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_defines.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_dmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_exp_board.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_gi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_io_board.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_port_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_segment_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_servo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/fast/fast_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/i2c_servo_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.289872 mpf-0.57.1.dev4/mpf/platforms/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/accelerometer_platform_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/dmd_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/driver_platform_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/hardware_sound_platform_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/i2c_platform_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/light_platform_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/segment_display_platform_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/servo_platform_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/stepper_platform_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/interfaces/switch_platform_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/light_segment_displays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.293872 mpf-0.57.1.dev4/mpf/platforms/lisy/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/lisy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/lisy/defines.py
--rw-r--r--   0 runner    (1001) docker     (127)    39151 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/lisy/lisy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/mma8451.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.293872 mpf-0.57.1.dev4/mpf/platforms/mypinballs/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/mypinballs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/mypinballs/mypinballs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/openpixel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.293872 mpf-0.57.1.dev4/mpf/platforms/opp/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/opp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55210 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/opp/opp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10709 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/opp/opp_coil.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/opp/opp_incand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/opp/opp_modern_lights.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/opp/opp_rs232_intf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/opp/opp_serial_communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/opp/opp_servo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/opp/opp_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/osc.py
--rw-r--r--   0 runner    (1001) docker     (127)    29212 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/p3_roc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/p_roc.py
--rw-r--r--   0 runner    (1001) docker     (127)    55913 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/p_roc_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/p_roc_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pin2dmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/platforms/pinproc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.293872 mpf-0.57.1.dev4/mpf/platforms/pinproc/osx/
--rwxr-xr-x   0 runner    (1001) docker     (127)   156500 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/osx/pinproc.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.297872 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/
--rw-r--r--   0 runner    (1001) docker     (127)    84273 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/pinproc.cp310-win32.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   102717 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/pinproc.cp310-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (127)    84318 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/pinproc.cp311-win32.pyd
--rw-r--r--   0 runner    (1001) docker     (127)   102773 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/pinproc.cp311-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (127)    54784 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/pinproc.cp312-win32.pyd
--rw-r--r--   0 runner    (1001) docker     (127)    68096 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/pinproc.cp312-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (127)    65536 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/pinproc.cp38-win32.pyd
--rw-r--r--   0 runner    (1001) docker     (127)    80896 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/pinproc.cp38-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (127)    54272 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/pinproc.cp39-win32.pyd
--rw-r--r--   0 runner    (1001) docker     (127)    68096 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pinproc/windows/pinproc.cp39-win_amd64.pyd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.297872 mpf-0.57.1.dev4/mpf/platforms/pkone/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pkone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30216 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pkone/pkone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_coil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_lights.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_lightshow.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_serial_communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_servo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.301872 mpf-0.57.1.dev4/mpf/platforms/pololu/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pololu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pololu/pololu_tic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pololu/pololu_ticcmd_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/pololu_maestro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.301872 mpf-0.57.1.dev4/mpf/platforms/rpi/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/rpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/rpi/rpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/rpi_dmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19845 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/smart_virtual.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/smartmatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/smbus2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/snux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/spi_bit_bang.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.301872 mpf-0.57.1.dev4/mpf/platforms/spike/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/spike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69460 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/spike/spike.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/spike/spike_defines.py
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/step_stick.py
--rw-r--r--   0 runner    (1001) docker     (127)    24849 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/system11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.301872 mpf-0.57.1.dev4/mpf/platforms/trinamics/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/trinamics/README
--rw-r--r--   0 runner    (1001) docker     (127)    30543 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/trinamics/TMCL.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/trinamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/trinamics_steprocker.py
--rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/virtual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.301872 mpf-0.57.1.dev4/mpf/platforms/virtual_pinball/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/virtual_pinball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/virtual_pinball/virtual_pinball.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.301872 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    56475 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/platform_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/platform_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.301872 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/protobuf/platform.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/visual_pinball_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.305872 mpf-0.57.1.dev4/mpf/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/plugins/auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/plugins/info_lights.py
--rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/plugins/platform_integration_test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/plugins/switch_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.305872 mpf-0.57.1.dev4/mpf/plugins/twitch/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/plugins/twitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/plugins/twitch/twitch_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/plugins/twitch_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/plugins/virtual_segment_display_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.333872 mpf-0.57.1.dev4/mpf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/MpfBcpTestCase.py
--rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/MpfDocTestCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/MpfFakeGameTestCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/MpfGameTestCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/MpfIntegrationDocTestCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/MpfMachineTestCase.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/MpfPlatformIntegrationTest.py
--rw-r--r--   0 runner    (1001) docker     (127)    36697 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/MpfTestCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/TestDataManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17846 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.225871 mpf-0.57.1.dev4/mpf/tests/machine_files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/tests/machine_files/accelerometer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.333872 mpf-0.57.1.dev4/mpf/tests/machine_files/accelerometer/config/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/accelerometer/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.333872 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/config/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/auto_select/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.333872 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/auto_select/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/auto_select/config/auto_select.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.333872 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/base/config/
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/base/config/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.333872 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/tests/machine_files/apc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.333872 mpf-0.57.1.dev4/mpf/tests/machine_files/apc/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/apc/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/config/test_asset_loading.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.177870 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/custom1/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/custom1/show8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/mode_start/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/mode_start/show9.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/on_demand/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/on_demand/show10.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/preload/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/preload/show7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/show6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/custom1/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/custom1/show11.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/custom1/show13.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/on_demand/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/on_demand/show5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/preload/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/preload/show4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/preload/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/preload/subfolder/show4b.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/show1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/show12.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/show2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/show3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/auditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/auditor/config/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/auditor/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/auditor/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/auditor/modes/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/auditor/modes/base/config/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/auditor/modes/base/config/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/autofire/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/autofire/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/autofire/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_controller/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.337873 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_controller/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_controller/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_controller/config/regression.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.341873 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_auto_manual_plunger.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_event_confirmation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_event_ejector.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_jam_switch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_jam_switch_initial.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_manual_with_target.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_no_plunger_switch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_routing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_switch_confirmation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_trigger_events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_enable_coil.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_enable_coil_multiple.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_gottlieb_trough.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_gottlieb_trough_with_initial_balls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_hold_coil.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_jam_and_ball_left.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_modern_trough_plunger_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_player_controlled_eject.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_playfield_lock.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_pulse_eject.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_single_device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_system_11_trough.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_system_11_trough_startup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_too_long_exit_count_delay.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/trough_entrance_switch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/trough_entrance_switch_initial_balls.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_holds/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.341873 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_holds/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_holds/config/test_ball_holds.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_holds/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_holds/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.341873 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_holds/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_holds/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_routing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_routing/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_routing/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_routing/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_routing/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_routing/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_routing/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/config/config_ball_device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/config/config_with_balls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/config/mechanical_eject.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/config/missing_initial.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/config/no_eject.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/config/multiple_connections_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/config/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.181871 mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/config/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/modes/mode3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/modes/mode3/config/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/blocking_events/modes/mode3/config/mode3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/config/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/modes/bonus/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/modes/bonus/config/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/modes/bonus/config/bonus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.345873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_additional_events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_additional_events/config/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_additional_events/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_additional_events/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_additional_events/modes/bonus/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_additional_events/modes/bonus/config/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_additional_events/modes/bonus/config/bonus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_additional_events/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_additional_events/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_additional_events/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/config/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/bonus/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/bonus/config/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/bonus/config/bonus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_no_keep_multiplier/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_no_keep_multiplier/config/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_no_keep_multiplier/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/bonus/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/bonus/config/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/bonus/config/bonus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/config/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.185871 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/blocking_carousel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/blocking_carousel/config/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/blocking_carousel/config/blocking_carousel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/carousel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/carousel/config/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/carousel/config/carousel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/conditional_carousel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/conditional_carousel/config/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/conditional_carousel/config/conditional_carousel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/second_carousel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/second_carousel/config/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/carousel/modes/second_carousel/config/second_carousel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/coil_player/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/coil_player/config/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/coil_player/config/coil_player.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/coil_player/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/coil_player/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/coil_player/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/coil_player/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/combo_switches/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/combo_switches/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/combo_switches/config/combo_switches.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/combo_switches/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/combo_switches/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/combo_switches/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/combo_switches/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_errors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_errors/broken_show/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_errors/broken_show/config/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_errors/broken_show/config/show.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_errors/broken_show/shows/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_errors/broken_show/shows/broken_show.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_interface/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_interface/config/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_interface/config/test_config_interface.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_interface/config/test_config_interface_missing_version.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_interface/config/test_config_interface_old_version.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.349873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/config/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/game/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/game/config/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/game/config/game.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/mode1/shows/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/mode1/shows/mode1_show.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/shows/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_loader/shows/show1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/config/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/config/test_config_players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/modes/mode1/shows/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/modes/mode1/shows/mode1_show.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.189870 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/shows/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_players/shows/show1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/config_processor/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_processor/typo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_processor/working.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/config_processor/working_subconfig.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/counters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/counters/config/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/counters/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/counters/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/counters/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/counters/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/counters/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/credits/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/credits/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/credits/config/config_credit_tiers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/credits/config/config_freeplay.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/credits/config/config_inhibit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/credits/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/credits/modes/credits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/credits/modes/credits/config/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/credits/modes/credits/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/custom_code/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/custom_code/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/custom_code/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/custom_code/code/test_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/custom_code/config/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/custom_code/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/data_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.353873 mpf-0.57.1.dev4/mpf/tests/machine_files/data_manager/config/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/data_manager/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/device/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.357873 mpf-0.57.1.dev4/mpf/tests/machine_files/device/config/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/device/config/coils.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/device/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/device/config/config_dual_wound_coil.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/device_collection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.357873 mpf-0.57.1.dev4/mpf/tests/machine_files/device_collection/config/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/device_collection/config/test_device_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/digital_output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.357873 mpf-0.57.1.dev4/mpf/tests/machine_files/digital_output/config/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/digital_output/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/digital_score_reels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.357873 mpf-0.57.1.dev4/mpf/tests/machine_files/digital_score_reels/config/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/digital_score_reels/config/test_digital_score_reels.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.357873 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/diverter_with_activation_events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/only_events_no_coils.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_activation_switch_and_eject_confirm_switch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_delayed_eject.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_diverter_auto_disable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_diverter_dual_wound_coil.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_diverter_with_switch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_eject_to_oposide_sides.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_eject_to_oposide_sides2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_hold_activation_time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_hold_no_activation_time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_missing_ball_at_source.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_pulsed_activation_time.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/dmd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.357873 mpf-0.57.1.dev4/mpf/tests/machine_files/dmd/config/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/dmd/config/testDmd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/dmd/config/testRgbDmd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/drop_targets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.357873 mpf-0.57.1.dev4/mpf/tests/machine_files/drop_targets/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/drop_targets/config/test_drop_targets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/drop_targets/config/test_multiple_drop_resets_on_startup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/drop_targets/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/drop_targets/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.357873 mpf-0.57.1.dev4/mpf/tests/machine_files/drop_targets/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/drop_targets/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.357873 mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/config/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/config/test_event_manager.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/modes/game_mode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.357873 mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/modes/game_mode/config/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/modes/game_mode/config/game_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/modes/test_mode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/modes/test_mode/config/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/modes/test_mode/config/test_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/config/test_event_player.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/config/test_queue_event_player.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/config/test_random_event_player.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.193871 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/extra_ball/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/extra_ball/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/extra_ball/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/extra_ball/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/extra_ball/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/extra_ball/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/extra_ball/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/audio.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/audio2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/dmd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/error_lights.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/exp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/nano.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/neuron.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/retro.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/seg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/flippers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/flippers/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/flippers/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/flippers/config/hold_no_eos.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/flippers/config/software_eos_repulse.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/game/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/game/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/game/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/game/config/config_with_balls.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/head2head/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/head2head/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/head2head/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score/config/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score/config/high_score.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score/modes/high_score/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.361873 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score/modes/high_score/config/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score/modes/high_score/config/high_score.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_reverse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_reverse/config/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_reverse/config/high_score.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_reverse/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_reverse/modes/high_score/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_reverse/modes/high_score/config/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_reverse/modes/high_score/config/high_score.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_vars/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_vars/config/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_vars/config/high_score.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_vars/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_vars/modes/high_score/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_vars/modes/high_score/config/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/high_score_vars/modes/high_score/config/high_score.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/i2c_servo_controller/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/i2c_servo_controller/config/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/i2c_servo_controller/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/info_lights/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/info_lights/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/info_lights/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/kickback/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/kickback/config/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/kickback/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/light/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/light/config/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light/config/light.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light/config/light_default_color_correction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light/config/light_groups.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light/config/lights_on_drivers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light/config/matrix_lights.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/config/light_player.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/config/light_player_named_colors.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.197871 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/shows/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/shows/show_ext1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/shows/show_ext2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/shows/show_ext3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/light_segment_displays/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/light_segment_displays/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light_segment_displays/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/light_segment_displays/config/config_dots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/lisy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/lisy/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/lisy/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/lisy/config/config_modern.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/lisy/config/config_system11.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.365873 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode3/config/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode3/config/mode3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode4/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode4/config/mode4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/machine_vars/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/machine_vars/config/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/machine_vars/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/magnet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/magnet/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/magnet/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/match_mode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/match_mode/config/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/match_mode/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/match_mode/config/config_highscore.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/match_mode/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/match_mode/modes/match/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/match_mode/modes/match/config/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/match_mode/modes/match/config/match.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/mma8451/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/mma8451/config/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mma8451/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/config/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/config/test_broken_mode_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/config/test_empty_modes_section.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/config/test_loading_invalid_modes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/config/test_missing_mode_section.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/config/test_mode_without_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/config/test_modes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/config/test_modes_in_game.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/broken_mode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/broken_mode/config/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/broken_mode/config/broken_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/broken_mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/broken_mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/broken_mode2/config/broken_mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode1/config/mode1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode1/config/test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode3/code/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode3/code/mode3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode3/config/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode3/config/mode3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.201871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.369873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode4/config/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode4/config/mode4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/config/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/config/mode5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/config/test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/mode8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/mode8/config/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/mode8/config/mode8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/mode8/config/test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode6/config/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode6/config/mode6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode6/config/test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode7/config/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode7/config/mode7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode7/config/test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_restart_on_next_ball/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_restart_on_next_ball/config/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_restart_on_next_ball/config/mode_restart_on_next_ball.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_without_config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_without_config/config/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mode_tests/modes/mode_without_config/config/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/motor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/motor/config/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/motor/config/drop_target.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/motor/config/ghostbusters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/motor/config/multiposition_motor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/motor/config/multiposition_motor_home_in_the_middle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/motor/config/multiposition_motor_start_on_end_switch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/mpftestcase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/mpftestcase/config/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mpftestcase/config/test_mpftestcase.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode3/config/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode3/config/mode3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode4/config/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode4/config/mode4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.373873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode5/config/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode5/config/mode5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/config/testDefault.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/config/testMinVirtualPhysical.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/config/testNoVirtual.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/config/testPhysicalOnly.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/config/testPhysicalOnlyNoStealing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/config/testSourceDevices.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/config/testVirtualOnly.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/blocking/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/blocking/config/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/blocking/config/blocking.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/default/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/default/config/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/min_virtual_physical/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/min_virtual_physical/config/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/min_virtual_physical/config/min_virtual_physical.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.205871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/no_virtual/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/no_virtual/config/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/no_virtual/config/no_virtual.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/physical_only/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/physical_only/config/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/physical_only/config/physical_only.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/physical_only_no_stealing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/physical_only_no_stealing/config/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/physical_only_no_stealing/config/physical_only_no_stealing.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/source_devices/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/source_devices/config/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/source_devices/config/source_devices.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/virtual_only/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/virtual_only/config/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/virtual_only/config/virtual_only.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/mypinballs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/mypinballs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/mypinballs/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/null/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/null/config/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/null/config/null.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/openpixel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/openpixel/config/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/openpixel/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/openpixel/config/fadecandy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/opp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/opp/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/opp/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/opp/config/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/opp/config/config_stm32.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/osc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/osc/config/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/osc/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/p3_roc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/p3_roc/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/p3_roc/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/p_roc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.377873 mpf-0.57.1.dev4/mpf/tests/machine_files/p_roc/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/p_roc/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/p_roc/config/snux.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/p_roc/config/wpc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/pkone/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/pkone/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/pkone/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/platform/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/platform/config/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/platform/config/test_platform.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/platform/config/test_virtual.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/player_vars/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/player_vars/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/player_vars/config/player_vars.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/playfield/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/playfield/config/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/playfield/config/test_playfield.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/playfield_transfer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/playfield_transfer/config/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/playfield_transfer/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/config/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/config/plugin_config_player.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/modes/mode1/shows/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/modes/mode1/shows/show2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/modes/mode1/shows/show3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/shows/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/plugin_config_player/shows/show1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/pololu_maestro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/pololu_maestro/config/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/pololu_maestro/config/pololu_maestro.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.209871 mpf-0.57.1.dev4/mpf/tests/machine_files/pololu_tic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/pololu_tic/config/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/pololu_tic/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/randomizer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/randomizer/config/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/randomizer/config/randomizer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/rpi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/rpi/config/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/rpi/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/rpi_dmd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/rpi_dmd/config/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/rpi_dmd/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/score_queue/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/score_queue/config/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/score_queue/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/score_queue/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/score_queue/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/score_queue/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/score_queue/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/score_reels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/score_reels/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/score_reels/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/config/config_colors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/config/config_flashing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/config/config_transition.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/config/game.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/sequence_shot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/sequence_shot/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/sequence_shot/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/sequence_shot/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/sequence_shot/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/sequence_shot/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/sequence_shot/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/service_mode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.381873 mpf-0.57.1.dev4/mpf/tests/machine_files/service_mode/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/service_mode/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/servo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/servo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/servo/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/settings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/settings/config/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/settings/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/config/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/config/test_shot_group_rotate_with_exclude.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/config/test_shot_groups.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/config/test_shots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base/config/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base2/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base2/config/base2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base3/config/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base3/config/base3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.213871 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode3/config/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode3/config/mode3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/rotate_with_exclude/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/rotate_with_exclude/config/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/rotate_with_exclude/config/rotate_with_exclude.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/config/test_show_player_queue.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/config/test_show_pools.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/config/test_shows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/config/test_sync_ms.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode3/config/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode3/config/mode3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode4/config/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode4/config/mode4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.385873 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/8linesweep.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/myparentshow.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/on_demand/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/on_demand/mychildshow.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/test_show1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/test_show2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/test_show3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/test_show_key_token.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/test_variable_show.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/smart_matrix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/smart_matrix/config/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/smart_matrix/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/smart_matrix/config/old_cookie.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/smart_virtual_platform/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/smart_virtual_platform/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/smart_virtual_platform/config/test_coil_fired_plunger.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/smart_virtual_platform/config/test_entrance_switch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/smart_virtual_platform/config/test_smart_virtual.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/smart_virtual_platform/config/test_smart_virtual_initial.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/smbus2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/smbus2/config/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/smbus2/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/snux/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/snux/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/snux/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/spi_bit_bang/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/spi_bit_bang/config/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/spi_bit_bang/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/spike/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/spike/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/spike/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/spinners/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/spinners/config/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/spinners/config/test_spinners.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/config/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/modes/game_mode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/modes/game_mode/config/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/modes/game_mode/config/game_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/modes/non_game_mode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/modes/non_game_mode/config/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/modes/non_game_mode/config/non_game_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/step_stick/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/step_stick/config/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/step_stick/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/stepper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/stepper/config/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/stepper/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.217871 mpf-0.57.1.dev4/mpf/tests/machine_files/switch_controller/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/switch_controller/config/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/switch_controller/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/switch_player/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/switch_player/config/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/switch_player/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/config/config_mechanical_eject.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/config/config_system_11_trough.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/config/settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/modes/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/modes/base/config/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/modes/base/config/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/modes/tilt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/modes/tilt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/modes/tilt/config/tilt.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt_defaults/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt_defaults/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/tilt_defaults/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/timed_switches/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.389873 mpf-0.57.1.dev4/mpf/tests/machine_files/timed_switches/config/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/timed_switches/config/timed_switches.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/timed_switches/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/timed_switches/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/timed_switches/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/timed_switches/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/timer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/timer/config/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/timer/config/test_timer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/timer/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/timer/modes/mode_with_timers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/timer/modes/mode_with_timers/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/timer/modes/mode_with_timers/config/mode_with_timers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/timer/modes/mode_with_timers2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/timer/modes/mode_with_timers2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/timer/modes/mode_with_timers2/config/mode_with_timers2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/trinamics_steprocker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/trinamics_steprocker/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/trinamics_steprocker/config/trinamics_steprocker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/twitch_client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/twitch_client/config/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/twitch_client/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/config/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode1/config/mode1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode2/config/mode2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode3/config/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode3/config/mode3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode_for_logic_block/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode_for_logic_block/config/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode_for_logic_block/config/mode_for_logic_block.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.221871 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/non_game_mode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/non_game_mode/config/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/non_game_mode/config/non_game_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.225871 mpf-0.57.1.dev4/mpf/tests/machine_files/virtual_pinball/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/virtual_pinball/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/virtual_pinball/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.225871 mpf-0.57.1.dev4/mpf/tests/machine_files/virtual_segment_display_connector/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/virtual_segment_display_connector/config/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/virtual_segment_display_connector/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.225871 mpf-0.57.1.dev4/mpf/tests/machine_files/vpe/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/vpe/config/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/vpe/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.225871 mpf-0.57.1.dev4/mpf/tests/machine_files/vpx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/machine_files/vpx/config/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/machine_files/vpx/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)    14078 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/platforms/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/platforms/pinproc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/tests/regression_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/regression_tests/light_player_subscriptions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/regression_tests/shot_same_show_differnent_token.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/regression_tests/shots_with_token_in_profile_and_shot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/regression_tests/show_player_subscriptions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Accelerometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Achievement.py
--rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_AssetManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Attract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Autofire.py
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallController.py
--rw-r--r--   0 runner    (1001) docker     (127)    81566 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceAutoManualPlunger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceEnableCoil.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceEventConfirmation.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceEventEjector.py
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceHoldCoil.py
--rw-r--r--   0 runner    (1001) docker     (127)    35977 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceJamSwitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    43631 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceManualWithTarget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceModernTroughPlungerSetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceNoPlungerSwitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDevicePlayfieldLock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDevicePulseEject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceRouting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceSingle.py
--rw-r--r--   0 runner    (1001) docker     (127)    25763 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceSwitchConfirmation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10193 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDeviceTriggerEvents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallDevice_SmartVirtual.py
--rw-r--r--   0 runner    (1001) docker     (127)    24190 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallHold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallRouting.py
--rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallSave.py
--rw-r--r--   0 runner    (1001) docker     (127)    34236 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BallSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)    23083 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BcpInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BcpMc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BcpServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BcpSocketClient.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Blinkenlight.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_BlockingEvents.py
--rw-r--r--   0 runner    (1001) docker     (127)    14862 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Bonus.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_CarouselMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_CoilPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23960 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ComboSwitches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_CommandCreateConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    21152 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ConfigErrors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ConfigMissingVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ConfigOldVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ConfigPlayers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ConfigProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_CreditsMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_CustomCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DataManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Delay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DeviceCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DeviceDriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DeviceFlasher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DeviceGI.py
--rw-r--r--   0 runner    (1001) docker     (127)    22534 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DeviceLight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DeviceManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DeviceMatrixLight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DigitalOutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DigitalScoreReels.py
--rw-r--r--   0 runner    (1001) docker     (127)    24123 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Diverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Dmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    18577 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DropTargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_DualWoundCoil.py
--rw-r--r--   0 runner    (1001) docker     (127)    35867 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_EventManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_EventPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ExtraBall.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Fadecandy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Fast_Audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Fast_Dmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Fast_Exp.py
--rw-r--r--   0 runner    (1001) docker     (127)    33999 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Fast_Nano.py
--rw-r--r--   0 runner    (1001) docker     (127)    40125 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Fast_Neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Fast_Retro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Fast_Seg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Flippers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_FlippersHoldNoEos.py
--rw-r--r--   0 runner    (1001) docker     (127)    22876 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_FlippersSoftwareEosRepulse.py
--rw-r--r--   0 runner    (1001) docker     (127)    30362 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Game.py
--rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_GottliebTrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Head2Head.py
--rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_HighScoreMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_HighScoreModeWithVars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_I2cServoController.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_InfoLights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Kickback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_LightGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)    15265 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_LightPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_LightPositions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_LightSegmentDisplays.py
--rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Lisy.py
--rw-r--r--   0 runner    (1001) docker     (127)    35954 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_LogicBlocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_MMA8451.py
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_MachineVariables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Magnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_MatchMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ModesConfigValidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Motors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_MpfTestCase.py
--rw-r--r--   0 runner    (1001) docker     (127)    45871 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_MultiBall.py
--rw-r--r--   0 runner    (1001) docker     (127)    33392 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_MultiballLock.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_MyPinballs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35422 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_OPP.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Openpixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Osc.py
--rw-r--r--   0 runner    (1001) docker     (127)    55750 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_P3_Roc.py
--rw-r--r--   0 runner    (1001) docker     (127)    34632 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_PKONE.py
--rw-r--r--   0 runner    (1001) docker     (127)    36398 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_P_Roc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9048 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_PlaceholderManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_PlayerVars.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Playfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_PlayfieldTransfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_PluginConfigPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_PololuMaestro.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_PololuTic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_QueueEventPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_RGBColor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_RandomEventPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Randomizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Rpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_RpiDmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ScoreQueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    20158 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ScoreReels.py
--rw-r--r--   0 runner    (1001) docker     (127)    77415 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_SegmentDisplay.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_SegmentMappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_SequenceShot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ServiceCli.py
--rw-r--r--   0 runner    (1001) docker     (127)    24766 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ServiceMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Servo.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    18353 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ShotGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)    37428 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Shots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_ShowPools.py
--rw-r--r--   0 runner    (1001) docker     (127)    42012 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Shows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_SmartMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_SmartVirtualPlatform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Smbus2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Snux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_SpiBitBang.py
--rw-r--r--   0 runner    (1001) docker     (127)    73695 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Spike.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Spinners.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_StateMachine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_StepStick.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Stepper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11669 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_SwitchController.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_SwitchPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_SwitchPositions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_System11Trough.py
--rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Tilt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_TimedSwitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_TooLongExitCountDelay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_TrinamicsStepRocker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_TroughEntranceSwitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_TwitchClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Utility_Functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_VPX.py
--rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_VariablePlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_Virtual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_VirtualPinball.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_VirtualSegmentDisplayConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_VisualPinballEngine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/test_YamlInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/tests/vpe_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.393873 mpf-0.57.1.dev4/mpf/wire/
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/wire/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20521 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf/wire/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)    20225 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mpf-logo-200.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.397873 mpf-0.57.1.dev4/mpf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-22 22:07:04.000000 mpf-0.57.1.dev4/mpf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    46711 2024-04-22 22:07:05.000000 mpf-0.57.1.dev4/mpf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:07:04.000000 mpf-0.57.1.dev4/mpf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 22:07:04.000000 mpf-0.57.1.dev4/mpf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-22 22:07:04.000000 mpf-0.57.1.dev4/mpf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 22:07:04.000000 mpf-0.57.1.dev4/mpf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:07:05.397873 mpf-0.57.1.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/sonar-project.properties
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/test_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.397873 mpf-0.57.1.dev4/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)    13276 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/tools/afl_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/tools/afl_howto.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/tools/convert_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/tools/debug_run_game.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/tools/p3_switch_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:07:05.397873 mpf-0.57.1.dev4/tools/smart_matrix_dmd_teensy_code/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4019 2024-04-22 22:06:25.000000 mpf-0.57.1.dev4/tools/smart_matrix_dmd_teensy_code/smart_matrix_dmd_teensy_code.ino
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.339022 mpf-0.80.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/.bandit
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.155023 mpf-0.80.0.dev1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.159023 mpf-0.80.0.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/.github/workflows/build_wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/.github/workflows/prospector.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-25 20:45:59.339022 mpf-0.80.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.159023 mpf-0.80.0.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.159023 mpf-0.80.0.dev1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.159023 mpf-0.80.0.dev1/docs/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.163023 mpf-0.80.0.dev1/docs/_static/images/icons/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9820 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-114x114.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7640 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-120x120.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11750 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-144x144.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15171 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-152x152.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3769 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-57x57.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3533 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-60x60.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5111 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-72x72.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5829 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-76x76.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8488 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/favicon-128.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      637 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/favicon-16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23562 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/favicon-196x196.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1620 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/favicon-32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6167 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/favicon-96x96.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34494 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/favicon.ico
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11750 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/mstile-144x144.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30530 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/mstile-150x150.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    95427 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/mstile-310x150.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)   145659 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/mstile-310x310.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8488 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/icons/mstile-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20225 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/mpf-logo-200.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/mpf-logo-tiny.png
+-rw-r--r--   0 runner    (1001) docker     (127)   280785 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/images/mpf-logo-tiny@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_static/mpf.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.167023 mpf-0.80.0.dev1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/config_players.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/config_players_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/devices_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/machine.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/machine_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/misc_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/modes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/modes_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/platforms_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/self.machine.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/_templates/tests_overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.171023 mpf-0.80.0.dev1/docs/bcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/ball_end.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/ball_start.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/error.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/goodbye.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/hello.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/machine_variable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/mode_start.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/mode_stop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/monitor_start.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/monitor_stop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/player_added.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/player_turn_start.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/player_variable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/register_trigger.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/remove_trigger.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/reset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/reset_complete.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/switch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/bcp/trigger.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.171023 mpf-0.80.0.dev1/docs/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/code/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/code/machine_code.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/code/mode_code.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18834 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.171023 mpf-0.80.0.dev1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/dev/Send variables via self.machine.events.post.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/dev/dev_environment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/dev/event_annotations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/dev/hardware.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/dev/mc.widget_player.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/dev/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.171023 mpf-0.80.0.dev1/docs/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/functions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/functions/machine_variables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/functions/player_variables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.175023 mpf-0.80.0.dev1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/images/custom_mode_code.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14947 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/images/scriptlet.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81139 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/images/test_classes.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.175023 mpf-0.80.0.dev1/docs/overview/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/overview/boot_process.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/overview/files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/overview/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/overview/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/overview/yaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.175023 mpf-0.80.0.dev1/docs/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/testing/fuzz_testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/testing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/testing/running_mpf_tests.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.175023 mpf-0.80.0.dev1/docs/testing/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/testing/tutorial/1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/testing/tutorial/2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/testing/writing_machine_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/docs/testing/writing_mpf_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.175023 mpf-0.80.0.dev1/mpf/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.179023 mpf-0.80.0.dev1/mpf/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31019 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/assets/show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.179023 mpf-0.80.0.dev1/mpf/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.095023 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.095023 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.179023 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/events/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/events/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.095023 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/shows/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.179023 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/shows/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/shows/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.179023 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/shows/shows/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/shows/shows/minimal_light_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/shows/shows/minimal_light_show_token.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/shows/shows/multi_step_tags.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/shows/shows/single_step_tag.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.095023 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/switch_hits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.179023 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/switch_hits/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/machine_files/switch_hits/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/test_benchmark_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/test_benchmark_light_shows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/benchmarks/test_benchmark_switch_hits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.183023 mpf-0.80.0.dev1/mpf/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/both.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/create_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9472 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/logging_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/commands/wire.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.187023 mpf-0.80.0.dev1/mpf/config_players/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/bcp_plugin_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/blinkenlight_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/block_event_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/coil_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/device_config_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/event_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/flasher_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/flat_config_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/hardware_sound_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/light_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/plugin_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/queue_event_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/queue_relay_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/random_event_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/score_queue_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/segment_display_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/show_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/slide_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/sound_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/variable_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_players/widget_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81029 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/config_spec.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.195023 mpf-0.80.0.dev1/mpf/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40488 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/async_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/ball_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/ball_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.195023 mpf-0.80.0.dev1/mpf/core/bcp/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/bcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/bcp/bcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/bcp/bcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36057 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/bcp/bcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/bcp/bcp_pickle_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/bcp/bcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/bcp/bcp_socket_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/bcp/bcp_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/case_insensitive_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13080 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16343 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/config_player.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11216 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/config_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/config_spec_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29482 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/crash_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/custom_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/delays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/device_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/enable_disable_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40793 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/file_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/light_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39389 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/machine_vars.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23375 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/mode_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/mode_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/mpf_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/placeholder_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/platform_batch_light_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23725 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/platform_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/randomizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21671 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/rgb_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/rgba_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66242 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/segment_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/service_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/settings_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/show_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30374 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/switch_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/system_wide_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18930 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/text_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30290 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/core/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.207023 mpf-0.80.0.dev1/mpf/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/accelerometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/achievement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/achievement_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/autofire.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.207023 mpf-0.80.0.dev1/mpf/devices/ball_device/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/ball_count_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28823 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/ball_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/ball_device_ejector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/ball_device_state_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/default_ball_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/enable_coil_ejector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/entrance_switch_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/event_ejector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/hold_coil_ejector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/incoming_balls_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27532 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/outgoing_balls_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/physical_ball_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/pulse_coil_ejector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_device/switch_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_hold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/ball_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/blinkenlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/combo_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/device_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/digital_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/digital_score_reel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/diverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/dmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18753 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19396 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/drop_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/dual_wound_coil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/extra_ball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/extra_ball_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/flipper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/hardware_sound_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/kickback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36761 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/light_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23267 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/logic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/multiball.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/multiball_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16670 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/playfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/playfield_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/power_supply_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/rgb_dmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/score_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/score_reel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/score_reel_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/score_reel_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/devices/segment_display/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/segment_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18898 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/segment_display/segment_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/segment_display/segment_display_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/segment_display/text_stack_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/segment_display/transition_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22277 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/segment_display/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/sequence_shot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/servo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19220 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/shot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/shot_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/shot_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/show_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/speedometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/stepper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/timed_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21260 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/devices/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/exceptions/base_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/exceptions/config_file_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/exceptions/driver_limits_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/exceptions/runtime_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/file_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/file_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/file_interfaces/pickle_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/file_interfaces/yaml_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/modes/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/modes/attract/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/attract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/modes/attract/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/attract/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/attract/code/attract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/modes/attract/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/attract/config/attract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/modes/bonus/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/bonus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/modes/bonus/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/bonus/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/bonus/code/bonus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/modes/bonus/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/bonus/config/bonus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.211023 mpf-0.80.0.dev1/mpf/modes/carousel/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/carousel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/carousel/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/carousel/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/carousel/code/carousel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/credits/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/credits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/credits/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/credits/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27935 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/credits/code/credits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/credits/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/credits/config/credits.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/game/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/game/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/game/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/game/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31533 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/game/code/game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/game/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/game/config/game.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/high_score/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/high_score/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/high_score/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/high_score/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/high_score/code/high_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/high_score/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/high_score/config/high_score.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/high_score/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/high_score/images/back_arrow_7x7.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/high_score/images/back_arrow_7x7_selected.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/high_score/images/end_11x7.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/high_score/images/end_11x7_selected.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.099023 mpf-0.80.0.dev1/mpf/modes/match/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/match/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/match/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/match/code/match.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/match/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/match/config/match.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.215023 mpf-0.80.0.dev1/mpf/modes/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.219023 mpf-0.80.0.dev1/mpf/modes/service/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34256 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/service/code/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.219023 mpf-0.80.0.dev1/mpf/modes/service/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/service/config/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.219023 mpf-0.80.0.dev1/mpf/modes/service/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/service/sounds/power_off.ogg
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/service/sounds/switch_hit.ogg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.099023 mpf-0.80.0.dev1/mpf/modes/service_dmd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.219023 mpf-0.80.0.dev1/mpf/modes/service_dmd/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/service_dmd/config/service_dmd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.099023 mpf-0.80.0.dev1/mpf/modes/service_segment_display/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.219023 mpf-0.80.0.dev1/mpf/modes/service_segment_display/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/service_segment_display/config/service_segment_display.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.219023 mpf-0.80.0.dev1/mpf/modes/tilt/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/tilt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.219023 mpf-0.80.0.dev1/mpf/modes/tilt/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/tilt/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/tilt/code/tilt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.219023 mpf-0.80.0.dev1/mpf/modes/tilt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/modes/tilt/config/tilt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/mpfconfig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.219023 mpf-0.80.0.dev1/mpf/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/parsers/event_reference_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/parsers/special_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.223023 mpf-0.80.0.dev1/mpf/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/base_serial_communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/driver_light_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fadecandy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.227023 mpf-0.80.0.dev1/mpf/platforms/fast/
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.227023 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/aud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/dmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/emu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/net_nano.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13610 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/net_neuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/net_retro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/communicators/seg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38995 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_defines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_dmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_exp_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_gi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_io_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_port_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_segment_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_servo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/fast/fast_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/i2c_servo_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.231023 mpf-0.80.0.dev1/mpf/platforms/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/accelerometer_platform_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/dmd_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/driver_platform_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/hardware_sound_platform_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/i2c_platform_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/light_platform_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/segment_display_platform_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/servo_platform_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/stepper_platform_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/interfaces/switch_platform_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/light_segment_displays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.231023 mpf-0.80.0.dev1/mpf/platforms/lisy/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/lisy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/lisy/defines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39151 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/lisy/lisy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/mma8451.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.231023 mpf-0.80.0.dev1/mpf/platforms/mypinballs/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/mypinballs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/mypinballs/mypinballs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/openpixel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.231023 mpf-0.80.0.dev1/mpf/platforms/opp/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/opp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55210 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/opp/opp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10709 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/opp/opp_coil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/opp/opp_incand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/opp/opp_modern_lights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/opp/opp_rs232_intf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/opp/opp_serial_communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/opp/opp_servo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/opp/opp_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/osc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29212 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/p3_roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/p_roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55913 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/p_roc_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/p_roc_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pin2dmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.103023 mpf-0.80.0.dev1/mpf/platforms/pinproc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.231023 mpf-0.80.0.dev1/mpf/platforms/pinproc/osx/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   156500 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/osx/pinproc.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.235023 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)    84273 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/pinproc.cp310-win32.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   102717 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/pinproc.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)    84318 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/pinproc.cp311-win32.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)   102773 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/pinproc.cp311-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)    54784 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/pinproc.cp312-win32.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)    68096 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/pinproc.cp312-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)    65536 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/pinproc.cp38-win32.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)    80896 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/pinproc.cp38-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)    54272 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/pinproc.cp39-win32.pyd
+-rw-r--r--   0 runner    (1001) docker     (127)    68096 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pinproc/windows/pinproc.cp39-win_amd64.pyd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.235023 mpf-0.80.0.dev1/mpf/platforms/pkone/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pkone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30216 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pkone/pkone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_coil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_lights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_lightshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_serial_communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_servo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.239023 mpf-0.80.0.dev1/mpf/platforms/pololu/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pololu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pololu/pololu_tic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pololu/pololu_ticcmd_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/pololu_maestro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.239023 mpf-0.80.0.dev1/mpf/platforms/rpi/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/rpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/rpi/rpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/rpi_dmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19845 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/smart_virtual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/smartmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/smbus2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/snux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/spi_bit_bang.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.239023 mpf-0.80.0.dev1/mpf/platforms/spike/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/spike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69460 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/spike/spike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/spike/spike_defines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/step_stick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24849 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/system11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.239023 mpf-0.80.0.dev1/mpf/platforms/trinamics/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/trinamics/README
+-rw-r--r--   0 runner    (1001) docker     (127)    30543 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/trinamics/TMCL.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/trinamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/trinamics_steprocker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/virtual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.239023 mpf-0.80.0.dev1/mpf/platforms/virtual_pinball/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/virtual_pinball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/virtual_pinball/virtual_pinball.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.239023 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56475 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/platform_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/platform_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.239023 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/protobuf/platform.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/visual_pinball_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.243023 mpf-0.80.0.dev1/mpf/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/plugins/auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/plugins/info_lights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/plugins/platform_integration_test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/plugins/switch_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.243023 mpf-0.80.0.dev1/mpf/plugins/twitch/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/plugins/twitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/plugins/twitch/twitch_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/plugins/twitch_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/plugins/virtual_segment_display_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.275023 mpf-0.80.0.dev1/mpf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/MpfBcpTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/MpfDocTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/MpfFakeGameTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/MpfGameTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/MpfIntegrationDocTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/MpfMachineTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/MpfPlatformIntegrationTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36697 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/MpfTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/TestDataManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17846 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.103023 mpf-0.80.0.dev1/mpf/tests/machine_files/accelerometer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.275023 mpf-0.80.0.dev1/mpf/tests/machine_files/accelerometer/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/accelerometer/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.103023 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.275023 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.103023 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.103023 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/auto_select/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.275023 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/auto_select/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/auto_select/config/auto_select.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.103023 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.275023 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/base/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/base/config/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.103023 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.275023 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.103023 mpf-0.80.0.dev1/mpf/tests/machine_files/apc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/apc/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/apc/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/config/test_asset_loading.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.103023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.103023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/custom1/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/custom1/show8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/mode_start/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/mode_start/show9.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/on_demand/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/on_demand/show10.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/preload/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/preload/show7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/show6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/custom1/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/custom1/show11.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/custom1/show13.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/on_demand/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/on_demand/show5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/preload/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/preload/show4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/preload/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/preload/subfolder/show4b.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/show1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/show12.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/show2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/show3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/auditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/auditor/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/auditor/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/auditor/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/auditor/modes/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/auditor/modes/base/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/auditor/modes/base/config/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/autofire/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/autofire/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/autofire/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_controller/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.279023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_controller/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_controller/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_controller/config/regression.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.283023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_auto_manual_plunger.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_event_confirmation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_event_ejector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_jam_switch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_jam_switch_initial.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_manual_with_target.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_no_plunger_switch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_routing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_switch_confirmation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_trigger_events.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_enable_coil.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_enable_coil_multiple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_gottlieb_trough.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_gottlieb_trough_with_initial_balls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_hold_coil.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_jam_and_ball_left.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_modern_trough_plunger_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_player_controlled_eject.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_playfield_lock.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_pulse_eject.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_single_device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_system_11_trough.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_system_11_trough_startup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_too_long_exit_count_delay.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/trough_entrance_switch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/trough_entrance_switch_initial_balls.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_holds/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_holds/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_holds/config/test_ball_holds.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_holds/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_holds/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_holds/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_holds/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_routing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_routing/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_routing/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_routing/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_routing/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_routing/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_routing/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/config/config_ball_device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/config/config_with_balls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/config/mechanical_eject.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/config/missing_initial.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/config/no_eject.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.107023 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/config/multiple_connections_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/modes/mode3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/modes/mode3/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/blocking_events/modes/mode3/config/mode3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/modes/bonus/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/modes/bonus/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/modes/bonus/config/bonus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.287023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_additional_events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_additional_events/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_additional_events/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_additional_events/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_additional_events/modes/bonus/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_additional_events/modes/bonus/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_additional_events/modes/bonus/config/bonus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_additional_events/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_additional_events/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_additional_events/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/bonus/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/bonus/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/bonus/config/bonus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.111023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_dynamic_keep_multiplier/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_no_keep_multiplier/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_no_keep_multiplier/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_no_keep_multiplier/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/bonus/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/bonus/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/bonus/config/bonus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/bonus_no_keep_multiplier/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/blocking_carousel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/blocking_carousel/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/blocking_carousel/config/blocking_carousel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/carousel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/carousel/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/carousel/config/carousel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/conditional_carousel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/conditional_carousel/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/conditional_carousel/config/conditional_carousel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/second_carousel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/second_carousel/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/carousel/modes/second_carousel/config/second_carousel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/coil_player/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/coil_player/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/coil_player/config/coil_player.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/coil_player/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/coil_player/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/coil_player/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/coil_player/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/combo_switches/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/combo_switches/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/combo_switches/config/combo_switches.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/combo_switches/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/combo_switches/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/combo_switches/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/combo_switches/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_errors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_errors/broken_show/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_errors/broken_show/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_errors/broken_show/config/show.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_errors/broken_show/shows/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_errors/broken_show/shows/broken_show.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_interface/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_interface/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_interface/config/test_config_interface.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_interface/config/test_config_interface_missing_version.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_interface/config/test_config_interface_old_version.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/game/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/game/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/game/config/game.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.115023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.291023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/mode1/shows/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/mode1/shows/mode1_show.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/shows/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_loader/shows/show1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/config/test_config_players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/modes/mode1/shows/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/modes/mode1/shows/mode1_show.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/shows/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_players/shows/show1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/config_processor/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_processor/typo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_processor/working.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/config_processor/working_subconfig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/counters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/counters/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/counters/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/counters/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/counters/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/counters/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/counters/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/credits/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/credits/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/credits/config/config_credit_tiers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/credits/config/config_freeplay.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/credits/config/config_inhibit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/credits/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/credits/modes/credits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/credits/modes/credits/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/credits/modes/credits/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/custom_code/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/custom_code/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/custom_code/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/custom_code/code/test_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/custom_code/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/custom_code/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/data_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/data_manager/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/data_manager/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/device/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/device/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/device/config/coils.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/device/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/device/config/config_dual_wound_coil.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/device_collection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/device_collection/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/device_collection/config/test_device_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/digital_output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/digital_output/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/digital_output/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/digital_score_reels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.295023 mpf-0.80.0.dev1/mpf/tests/machine_files/digital_score_reels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/digital_score_reels/config/test_digital_score_reels.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.299023 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/diverter_with_activation_events.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/only_events_no_coils.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_activation_switch_and_eject_confirm_switch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_delayed_eject.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_diverter_auto_disable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_diverter_dual_wound_coil.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_diverter_with_switch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_eject_to_oposide_sides.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_eject_to_oposide_sides2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_hold_activation_time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_hold_no_activation_time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_missing_ball_at_source.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_pulsed_activation_time.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.119023 mpf-0.80.0.dev1/mpf/tests/machine_files/dmd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.299023 mpf-0.80.0.dev1/mpf/tests/machine_files/dmd/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/dmd/config/testDmd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/dmd/config/testRgbDmd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/drop_targets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.299023 mpf-0.80.0.dev1/mpf/tests/machine_files/drop_targets/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/drop_targets/config/test_drop_targets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/drop_targets/config/test_multiple_drop_resets_on_startup.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/drop_targets/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/drop_targets/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.299023 mpf-0.80.0.dev1/mpf/tests/machine_files/drop_targets/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/drop_targets/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.299023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/config/test_event_manager.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/modes/game_mode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.299023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/modes/game_mode/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/modes/game_mode/config/game_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/modes/test_mode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.299023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/modes/test_mode/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/modes/test_mode/config/test_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.299023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/config/test_event_player.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/config/test_queue_event_player.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/config/test_random_event_player.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.299023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.299023 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/extra_ball/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/extra_ball/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/extra_ball/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/extra_ball/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/extra_ball/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/extra_ball/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/extra_ball/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/audio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/audio2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/dmd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/error_lights.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/exp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/nano.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/neuron.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/retro.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/seg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/flippers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/flippers/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/flippers/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/flippers/config/hold_no_eos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/flippers/config/software_eos_repulse.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/game/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/game/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/game/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/game/config/config_with_balls.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/head2head/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/head2head/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/head2head/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score/config/high_score.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score/modes/high_score/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score/modes/high_score/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score/modes/high_score/config/high_score.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_reverse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_reverse/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_reverse/config/high_score.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_reverse/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.123023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_reverse/modes/high_score/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_reverse/modes/high_score/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_reverse/modes/high_score/config/high_score.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_vars/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_vars/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_vars/config/high_score.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_vars/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_vars/modes/high_score/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_vars/modes/high_score/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/high_score_vars/modes/high_score/config/high_score.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/i2c_servo_controller/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/i2c_servo_controller/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/i2c_servo_controller/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/info_lights/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/info_lights/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/info_lights/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/kickback/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.303023 mpf-0.80.0.dev1/mpf/tests/machine_files/kickback/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/kickback/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/light/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/light/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light/config/light.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light/config/light_default_color_correction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light/config/light_groups.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light/config/lights_on_drivers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light/config/matrix_lights.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/config/light_player.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/config/light_player_named_colors.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/shows/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/shows/show_ext1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/shows/show_ext2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/shows/show_ext3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/light_segment_displays/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/light_segment_displays/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light_segment_displays/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/light_segment_displays/config/config_dots.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/lisy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/lisy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/lisy/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/lisy/config/config_modern.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/lisy/config/config_system11.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode3/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode3/config/mode3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode4/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode4/config/mode4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/machine_vars/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/machine_vars/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/machine_vars/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.127023 mpf-0.80.0.dev1/mpf/tests/machine_files/magnet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/magnet/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/magnet/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/match_mode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/match_mode/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/match_mode/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/match_mode/config/config_highscore.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/match_mode/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/match_mode/modes/match/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/match_mode/modes/match/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/match_mode/modes/match/config/match.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mma8451/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.307023 mpf-0.80.0.dev1/mpf/tests/machine_files/mma8451/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mma8451/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/config/test_broken_mode_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/config/test_empty_modes_section.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/config/test_loading_invalid_modes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/config/test_missing_mode_section.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/config/test_mode_without_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/config/test_modes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/config/test_modes_in_game.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/broken_mode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/broken_mode/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/broken_mode/config/broken_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/broken_mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/broken_mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/broken_mode2/config/broken_mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode1/config/mode1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode1/config/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode3/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode3/code/mode3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode3/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode3/config/mode3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode4/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode4/config/mode4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/config/mode5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/config/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/mode8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/mode8/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/mode8/config/mode8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/mode5/mode8/config/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode6/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode6/config/mode6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode6/config/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode7/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode7/config/mode7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_in_sub_folder/sub_mode/mode7/config/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_restart_on_next_ball/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_restart_on_next_ball/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_restart_on_next_ball/config/mode_restart_on_next_ball.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_without_config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.311023 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_without_config/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mode_tests/modes/mode_without_config/config/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/motor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/motor/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/motor/config/drop_target.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/motor/config/ghostbusters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/motor/config/multiposition_motor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/motor/config/multiposition_motor_home_in_the_middle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/motor/config/multiposition_motor_start_on_end_switch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.131023 mpf-0.80.0.dev1/mpf/tests/machine_files/mpftestcase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/mpftestcase/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mpftestcase/config/test_mpftestcase.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode3/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode3/config/mode3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode4/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode4/config/mode4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode5/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode5/config/mode5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/config/testDefault.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/config/testMinVirtualPhysical.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/config/testNoVirtual.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/config/testPhysicalOnly.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/config/testPhysicalOnlyNoStealing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/config/testSourceDevices.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/config/testVirtualOnly.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/blocking/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/blocking/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/blocking/config/blocking.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/default/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/default/config/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/min_virtual_physical/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/min_virtual_physical/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/min_virtual_physical/config/min_virtual_physical.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/no_virtual/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/no_virtual/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/no_virtual/config/no_virtual.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/physical_only/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/physical_only/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/physical_only/config/physical_only.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/physical_only_no_stealing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/physical_only_no_stealing/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/physical_only_no_stealing/config/physical_only_no_stealing.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/source_devices/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/source_devices/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/source_devices/config/source_devices.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/virtual_only/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/virtual_only/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/virtual_only/config/virtual_only.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/mypinballs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.315023 mpf-0.80.0.dev1/mpf/tests/machine_files/mypinballs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/mypinballs/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/null/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/null/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/null/config/null.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/openpixel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/openpixel/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/openpixel/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/openpixel/config/fadecandy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.135023 mpf-0.80.0.dev1/mpf/tests/machine_files/opp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/opp/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/opp/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/opp/config/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/opp/config/config_stm32.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/osc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/osc/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/osc/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/p3_roc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/p3_roc/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/p3_roc/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/p_roc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/p_roc/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/p_roc/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/p_roc/config/snux.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/p_roc/config/wpc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/pkone/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/pkone/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/pkone/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/platform/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/platform/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/platform/config/test_platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/platform/config/test_virtual.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/player_vars/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/player_vars/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/player_vars/config/player_vars.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/playfield/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/playfield/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/playfield/config/test_playfield.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/playfield_transfer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/playfield_transfer/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/playfield_transfer/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/config/plugin_config_player.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/modes/mode1/shows/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/modes/mode1/shows/show2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/modes/mode1/shows/show3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/shows/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/plugin_config_player/shows/show1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/pololu_maestro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/pololu_maestro/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/pololu_maestro/config/pololu_maestro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/pololu_tic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/pololu_tic/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/pololu_tic/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/randomizer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/randomizer/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/randomizer/config/randomizer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/rpi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/rpi/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/rpi/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/rpi_dmd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/rpi_dmd/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/rpi_dmd/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/score_queue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.319023 mpf-0.80.0.dev1/mpf/tests/machine_files/score_queue/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/score_queue/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/score_queue/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/score_queue/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/score_queue/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/score_queue/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.139023 mpf-0.80.0.dev1/mpf/tests/machine_files/score_reels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/score_reels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/score_reels/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/config/config_colors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/config/config_flashing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/config/config_transition.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/config/game.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/sequence_shot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/sequence_shot/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/sequence_shot/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/sequence_shot/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/sequence_shot/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/sequence_shot/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/sequence_shot/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/service_mode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/service_mode/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/service_mode/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/servo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/servo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/servo/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/settings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/settings/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/settings/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/config/test_shot_group_rotate_with_exclude.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/config/test_shot_groups.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/config/test_shots.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base/config/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base2/config/base2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base3/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base3/config/base3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode3/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode3/config/mode3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/rotate_with_exclude/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.323023 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/rotate_with_exclude/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/rotate_with_exclude/config/rotate_with_exclude.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/config/test_show_player_queue.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/config/test_show_pools.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/config/test_shows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/config/test_sync_ms.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.143023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode3/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode3/config/mode3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode4/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode4/config/mode4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/8linesweep.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/myparentshow.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/on_demand/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/on_demand/mychildshow.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/test_show1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/test_show2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/test_show3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/test_show_key_token.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/test_variable_show.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/smart_matrix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/smart_matrix/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/smart_matrix/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/smart_matrix/config/old_cookie.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/smart_virtual_platform/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/smart_virtual_platform/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/smart_virtual_platform/config/test_coil_fired_plunger.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/smart_virtual_platform/config/test_entrance_switch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/smart_virtual_platform/config/test_smart_virtual.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/smart_virtual_platform/config/test_smart_virtual_initial.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/smbus2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/smbus2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/smbus2/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/snux/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/snux/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/snux/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/spi_bit_bang/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/spi_bit_bang/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/spi_bit_bang/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/spike/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/spike/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/spike/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/spinners/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/spinners/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/spinners/config/test_spinners.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/modes/game_mode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/modes/game_mode/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/modes/game_mode/config/game_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/modes/non_game_mode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.327023 mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/modes/non_game_mode/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/modes/non_game_mode/config/non_game_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/step_stick/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/step_stick/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/step_stick/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/stepper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/stepper/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/stepper/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/switch_controller/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/switch_controller/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/switch_controller/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/switch_player/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/switch_player/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/switch_player/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/config/config_mechanical_eject.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/config/config_system_11_trough.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/config/settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/modes/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/modes/base/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/modes/base/config/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.147023 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/modes/tilt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/modes/tilt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/modes/tilt/config/tilt.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt_defaults/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt_defaults/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/tilt_defaults/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/timed_switches/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/timed_switches/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/timed_switches/config/timed_switches.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/timed_switches/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/timed_switches/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/timed_switches/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/timed_switches/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/timer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/timer/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/timer/config/test_timer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/timer/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/timer/modes/mode_with_timers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/timer/modes/mode_with_timers/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/timer/modes/mode_with_timers/config/mode_with_timers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/timer/modes/mode_with_timers2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/timer/modes/mode_with_timers2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/timer/modes/mode_with_timers2/config/mode_with_timers2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/trinamics_steprocker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/trinamics_steprocker/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/trinamics_steprocker/config/trinamics_steprocker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/twitch_client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/twitch_client/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/twitch_client/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode1/config/mode1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode2/config/mode2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode3/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode3/config/mode3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode_for_logic_block/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode_for_logic_block/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode_for_logic_block/config/mode_for_logic_block.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/non_game_mode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/non_game_mode/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/non_game_mode/config/non_game_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/virtual_pinball/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/virtual_pinball/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/virtual_pinball/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/virtual_segment_display_connector/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/virtual_segment_display_connector/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/virtual_segment_display_connector/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/vpe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.331023 mpf-0.80.0.dev1/mpf/tests/machine_files/vpe/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/vpe/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.151023 mpf-0.80.0.dev1/mpf/tests/machine_files/vpx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.335023 mpf-0.80.0.dev1/mpf/tests/machine_files/vpx/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/machine_files/vpx/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.335023 mpf-0.80.0.dev1/mpf/tests/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)    14078 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/platforms/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/platforms/pinproc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.335023 mpf-0.80.0.dev1/mpf/tests/regression_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/regression_tests/light_player_subscriptions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/regression_tests/shot_same_show_differnent_token.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/regression_tests/shots_with_token_in_profile_and_shot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/regression_tests/show_player_subscriptions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Accelerometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Achievement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_AssetManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Attract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Autofire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallController.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81566 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceAutoManualPlunger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceEnableCoil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceEventConfirmation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceEventEjector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceHoldCoil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35977 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceJamSwitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43631 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceManualWithTarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceModernTroughPlungerSetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceNoPlungerSwitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDevicePlayfieldLock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDevicePulseEject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceRouting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceSingle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25763 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceSwitchConfirmation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10193 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDeviceTriggerEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallDevice_SmartVirtual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24190 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallHold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallRouting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallSave.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34236 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BallSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23083 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BcpInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BcpMc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BcpServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BcpSocketClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Blinkenlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_BlockingEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15536 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Bonus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_CarouselMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_CoilPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23960 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ComboSwitches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_CommandCreateConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21152 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ConfigErrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ConfigMissingVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ConfigOldVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ConfigPlayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ConfigProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_CreditsMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_CustomCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DataManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DeviceCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DeviceDriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DeviceFlasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DeviceGI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22534 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DeviceLight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DeviceManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DeviceMatrixLight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DigitalOutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DigitalScoreReels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24123 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Diverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Dmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18577 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DropTargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_DualWoundCoil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35867 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_EventManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_EventPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ExtraBall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Fadecandy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Fast_Audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Fast_Dmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Fast_Exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33999 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Fast_Nano.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40125 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Fast_Neuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Fast_Retro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Fast_Seg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Flippers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_FlippersHoldNoEos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22876 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_FlippersSoftwareEosRepulse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30362 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Game.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_GottliebTrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Head2Head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27962 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_HighScoreMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_HighScoreModeWithVars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_I2cServoController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_InfoLights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Kickback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_LightGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15265 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_LightPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_LightPositions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_LightSegmentDisplays.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Lisy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35954 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_LogicBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_MMA8451.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_MachineVariables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Magnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_MatchMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ModesConfigValidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Motors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_MpfTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45871 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_MultiBall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33392 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_MultiballLock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_MyPinballs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35422 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_OPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Openpixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Osc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55750 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_P3_Roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34632 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_PKONE.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36398 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_P_Roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9048 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_PlaceholderManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_PlayerVars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Playfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_PlayfieldTransfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_PluginConfigPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_PololuMaestro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_PololuTic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_QueueEventPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_RGBColor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_RandomEventPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Randomizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Rpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_RpiDmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ScoreQueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20158 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ScoreReels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77415 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_SegmentDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_SegmentMappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_SequenceShot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ServiceCli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24766 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ServiceMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Servo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18353 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ShotGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37428 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Shots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_ShowPools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42012 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Shows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_SmartMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_SmartVirtualPlatform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Smbus2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Snux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_SpiBitBang.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73695 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Spike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Spinners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_StateMachine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_StepStick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Stepper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11669 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_SwitchController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_SwitchPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_SwitchPositions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_System11Trough.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Tilt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_TimedSwitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_TooLongExitCountDelay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_TrinamicsStepRocker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_TroughEntranceSwitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_TwitchClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Utility_Functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_VPX.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_VariablePlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_Virtual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_VirtualPinball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_VirtualSegmentDisplayConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_VisualPinballEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/test_YamlInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/tests/vpe_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.335023 mpf-0.80.0.dev1/mpf/wire/
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/wire/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20521 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf/wire/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20225 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf-logo-200.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.335023 mpf-0.80.0.dev1/mpf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-25 20:45:58.000000 mpf-0.80.0.dev1/mpf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    46826 2024-05-25 20:45:59.000000 mpf-0.80.0.dev1/mpf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 20:45:58.000000 mpf-0.80.0.dev1/mpf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 20:45:58.000000 mpf-0.80.0.dev1/mpf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-25 20:45:58.000000 mpf-0.80.0.dev1/mpf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-25 20:45:58.000000 mpf-0.80.0.dev1/mpf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mpf.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:45:59.339022 mpf-0.80.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/sonar-project.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/test_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.335023 mpf-0.80.0.dev1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13276 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/tools/afl_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/tools/afl_howto.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/tools/convert_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/tools/debug_run_game.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/tools/p3_switch_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:59.335023 mpf-0.80.0.dev1/tools/smart_matrix_dmd_teensy_code/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4019 2024-05-25 20:45:19.000000 mpf-0.80.0.dev1/tools/smart_matrix_dmd_teensy_code/smart_matrix_dmd_teensy_code.ino
```

### Comparing `mpf-0.57.1.dev4/.github/workflows/build_wheels.yml` & `mpf-0.80.0.dev1/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/.github/workflows/prospector.yml` & `mpf-0.80.0.dev1/.github/workflows/prospector.yml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/.github/workflows/run_tests.yml` & `mpf-0.80.0.dev1/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/.gitignore` & `mpf-0.80.0.dev1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 .installed.cfg
 *.egg
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
-*.spec
+# AVW: Going to include the spec at least for reference
+.spec
 
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
```

### Comparing `mpf-0.57.1.dev4/.prospector.yaml` & `mpf-0.80.0.dev1/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/AUTHORS.md` & `mpf-0.80.0.dev1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/LICENSE.md` & `mpf-0.80.0.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/PKG-INFO` & `mpf-0.80.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpf
-Version: 0.57.1.dev4
+Version: 0.80.0.dev1
 Summary: The Mission Pinball Framework (MPF)
 Author-email: The Mission Pinball Framework Team <brian@missionpinball.org>
 License: MIT
 Project-URL: homepage, https://missionpinball.org
 Project-URL: support-forum, https://missionpinball.org/community/
 Keywords: pinball
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mpf-0.57.1.dev4/README.md` & `mpf-0.80.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/Makefile` & `mpf-0.80.0.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-114x114.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-120x120.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-144x144.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-152x152.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-57x57.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-60x60.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-72x72.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/apple-touch-icon-76x76.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/favicon-128.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/favicon-128.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/favicon-16x16.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/favicon-196x196.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/favicon-196x196.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/favicon-32x32.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/favicon-96x96.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/favicon.ico` & `mpf-0.80.0.dev1/docs/_static/images/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/mstile-144x144.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/mstile-150x150.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/mstile-310x150.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/mstile-310x310.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/icons/mstile-70x70.png` & `mpf-0.80.0.dev1/docs/_static/images/icons/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/mpf-logo-200.png` & `mpf-0.80.0.dev1/docs/_static/images/mpf-logo-200.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/mpf-logo-tiny.png` & `mpf-0.80.0.dev1/docs/_static/images/mpf-logo-tiny.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/images/mpf-logo-tiny@2x.png` & `mpf-0.80.0.dev1/docs/_static/images/mpf-logo-tiny@2x.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_static/mpf.css` & `mpf-0.80.0.dev1/docs/_static/mpf.css`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_templates/devices.rst` & `mpf-0.80.0.dev1/docs/_templates/devices.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_templates/devices_overview.rst` & `mpf-0.80.0.dev1/docs/_templates/devices_overview.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_templates/index.rst` & `mpf-0.80.0.dev1/docs/_templates/index.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_templates/modes.rst` & `mpf-0.80.0.dev1/docs/_templates/modes.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_templates/platforms.rst` & `mpf-0.80.0.dev1/docs/_templates/platforms.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/_templates/tests_overview.rst` & `mpf-0.80.0.dev1/docs/_templates/tests_overview.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/bcp/hello.rst` & `mpf-0.80.0.dev1/docs/bcp/hello.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/bcp/index.rst` & `mpf-0.80.0.dev1/docs/bcp/index.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/bcp/machine_variable.rst` & `mpf-0.80.0.dev1/docs/bcp/machine_variable.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/bcp/monitor_start.rst` & `mpf-0.80.0.dev1/docs/bcp/monitor_start.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/bcp/monitor_stop.rst` & `mpf-0.80.0.dev1/docs/bcp/monitor_stop.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/bcp/player_variable.rst` & `mpf-0.80.0.dev1/docs/bcp/player_variable.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/bcp/switch.rst` & `mpf-0.80.0.dev1/docs/bcp/switch.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/bcp/trigger.rst` & `mpf-0.80.0.dev1/docs/bcp/trigger.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/code/index.rst` & `mpf-0.80.0.dev1/docs/code/index.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/code/machine_code.rst` & `mpf-0.80.0.dev1/docs/code/machine_code.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/code/mode_code.rst` & `mpf-0.80.0.dev1/docs/code/mode_code.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/conf.py` & `mpf-0.80.0.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/dev/Send variables via self.machine.events.post.rst` & `mpf-0.80.0.dev1/docs/dev/Send variables via self.machine.events.post.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/dev/dev_environment.rst` & `mpf-0.80.0.dev1/docs/dev/dev_environment.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/dev/event_annotations.rst` & `mpf-0.80.0.dev1/docs/dev/event_annotations.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/dev/mc.widget_player.rst` & `mpf-0.80.0.dev1/docs/dev/mc.widget_player.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/functions/machine_variables.rst` & `mpf-0.80.0.dev1/docs/functions/machine_variables.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/functions/player_variables.rst` & `mpf-0.80.0.dev1/docs/functions/player_variables.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/images/custom_mode_code.png` & `mpf-0.80.0.dev1/docs/images/custom_mode_code.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/images/scriptlet.png` & `mpf-0.80.0.dev1/docs/images/scriptlet.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/images/test_classes.png` & `mpf-0.80.0.dev1/docs/images/test_classes.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/index.rst` & `mpf-0.80.0.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/make.bat` & `mpf-0.80.0.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/overview/boot_process.rst` & `mpf-0.80.0.dev1/docs/overview/boot_process.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/overview/files.rst` & `mpf-0.80.0.dev1/docs/overview/files.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/overview/installation.rst` & `mpf-0.80.0.dev1/docs/overview/installation.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/overview/yaml.rst` & `mpf-0.80.0.dev1/docs/overview/yaml.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/testing/index.rst` & `mpf-0.80.0.dev1/docs/testing/index.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/testing/running_mpf_tests.rst` & `mpf-0.80.0.dev1/docs/testing/running_mpf_tests.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/testing/tutorial/1.rst` & `mpf-0.80.0.dev1/docs/testing/tutorial/1.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/testing/tutorial/2.rst` & `mpf-0.80.0.dev1/docs/testing/tutorial/2.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/docs/testing/writing_machine_tests.rst` & `mpf-0.80.0.dev1/docs/testing/writing_machine_tests.rst`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/_version.py` & `mpf-0.80.0.dev1/mpf/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 It's used internally for all sorts of things, from printing the output of the
 `mpf --version` command, to making sure any processes connected via BCP are
 the proper versions, to automatically triggering new builds and deployments to
 PyPI.
 
 """
 
-__version__ = '0.57.1.dev4'  # Also consider whether MPF-MC pyproject.toml should be updated
+__version__ = '0.80.0.dev1'  # Also consider whether MPF-MC pyproject.toml should be updated
 '''The full version of MPF.'''
 
-__short_version__ = '0.57'
+__short_version__ = '0.80'
 '''The major.minor version of MPF.'''
 
 __bcp_version__ = '1.1'
 '''The version of BCP this build of MPF uses.'''
 
 __config_version__ = '6'
 '''The config file version this build of MPF uses.'''
```

### Comparing `mpf-0.57.1.dev4/mpf/assets/show.py` & `mpf-0.80.0.dev1/mpf/assets/show.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/benchmarks/machine_files/shows/config/config.yaml` & `mpf-0.80.0.dev1/mpf/benchmarks/machine_files/shows/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/benchmarks/test_benchmark_events.py` & `mpf-0.80.0.dev1/mpf/benchmarks/test_benchmark_events.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/benchmarks/test_benchmark_light_shows.py` & `mpf-0.80.0.dev1/mpf/benchmarks/test_benchmark_light_shows.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/benchmarks/test_benchmark_switch_hits.py` & `mpf-0.80.0.dev1/mpf/benchmarks/test_benchmark_switch_hits.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/commands/__init__.py` & `mpf-0.80.0.dev1/mpf/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/commands/both.py` & `mpf-0.80.0.dev1/mpf/commands/both.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/commands/build.py` & `mpf-0.80.0.dev1/mpf/commands/build.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/commands/create_config.py` & `mpf-0.80.0.dev1/mpf/commands/create_config.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/commands/diagnosis.py` & `mpf-0.80.0.dev1/mpf/commands/diagnosis.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/commands/game.py` & `mpf-0.80.0.dev1/mpf/commands/game.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,18 +156,18 @@
 
         try:
             os.makedirs(os.path.join(machine_path, 'logs'))
         except OSError as exception:
             if exception.errno != errno.EEXIST:
                 raise
 
-        full_logfile_path = os.path.join(machine_path, self.args.logfile)
+        self.args.full_logfile_path = os.path.join(machine_path, self.args.logfile)
 
         try:
-            os.remove(full_logfile_path)
+            os.remove(self.args.full_logfile_path)
         except OSError:
             pass
 
         if self.args.text_ui:
             console_log = logging.NullHandler()
             console_log.setLevel(logging.ERROR)
         else:
@@ -184,15 +184,15 @@
         console_log_queue = Queue()
         console_queue_handler = QueueHandler(console_log_queue)
         self.console_queue_listener = logging.handlers.QueueListener(
             console_log_queue, console_log, respect_handler_level=True)
         self.console_queue_listener.start()
 
         # initialize file log
-        file_log = logging.FileHandler(full_logfile_path)
+        file_log = logging.FileHandler(self.args.full_logfile_path)
         if self.args.jsonlogging:
             formatter = JSONFormatter()
         else:
             formatter = logging.Formatter('%(asctime)s : %(levelname)s : %(name)s : %(message)s')
         file_log.setFormatter(formatter)
 
         # initialize async handler for file log
@@ -269,14 +269,18 @@
         Cleanly shuts down logging and restores the console window if the Text
         UI option is used.
         """
         if exception:
             logging.exception(exception)
 
         logging.shutdown()
-        self.console_queue_listener.stop()
-        self.file_queue_listener.stop()
+        if self.console_queue_listener:
+            self.console_queue_listener.stop()
+            self.console_queue_listener = None
+        if self.file_queue_listener:
+            self.file_queue_listener.stop()
+            self.file_queue_listener = None
 
         if self.args.pause:
             input('Press ENTER to continue...')     # nosec
 
         sys.exit()
```

### Comparing `mpf-0.57.1.dev4/mpf/commands/hardware.py` & `mpf-0.80.0.dev1/mpf/commands/hardware.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/commands/logging_formatters.py` & `mpf-0.80.0.dev1/mpf/commands/logging_formatters.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/commands/service.py` & `mpf-0.80.0.dev1/mpf/commands/service.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/commands/test.py` & `mpf-0.80.0.dev1/mpf/commands/test.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/commands/wire.py` & `mpf-0.80.0.dev1/mpf/commands/wire.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/bcp_plugin_player.py` & `mpf-0.80.0.dev1/mpf/config_players/bcp_plugin_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/blinkenlight_player.py` & `mpf-0.80.0.dev1/mpf/config_players/blinkenlight_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/block_event_player.py` & `mpf-0.80.0.dev1/mpf/config_players/block_event_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/coil_player.py` & `mpf-0.80.0.dev1/mpf/config_players/coil_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/device_config_player.py` & `mpf-0.80.0.dev1/mpf/config_players/device_config_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/event_player.py` & `mpf-0.80.0.dev1/mpf/config_players/event_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/flasher_player.py` & `mpf-0.80.0.dev1/mpf/config_players/flasher_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/flat_config_player.py` & `mpf-0.80.0.dev1/mpf/config_players/flat_config_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/hardware_sound_player.py` & `mpf-0.80.0.dev1/mpf/config_players/hardware_sound_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/light_player.py` & `mpf-0.80.0.dev1/mpf/config_players/light_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/plugin_player.py` & `mpf-0.80.0.dev1/mpf/config_players/plugin_player.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,19 @@
         """Remove BCP events."""
         self.unload_player_events(self._show_keys[context + self.config_file_section])
         del self._show_keys[context + self.config_file_section]
         super().show_stop_callback(context)
 
     def play(self, settings, context, calling_context, priority=0, **kwargs):
         """Trigger remote player via BCP."""
+        # The triggering event's kwargs are passed through, and the triggering
+        # event may have come from BCP. Explicitly set _from_bcp=False so that
+        # this play event won't be swallowed.
+        if '_from_bcp' in kwargs:
+            del kwargs['_from_bcp']
         self.machine.bcp.interface.bcp_trigger(
             name='{}_play'.format(self.show_section),
             settings=settings, context=context, calling_context=calling_context,
             priority=priority, **kwargs)
 
     def clear_context(self, context):
         """Clear the context at remote player via BCP."""
```

### Comparing `mpf-0.57.1.dev4/mpf/config_players/queue_event_player.py` & `mpf-0.80.0.dev1/mpf/config_players/queue_event_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/queue_relay_player.py` & `mpf-0.80.0.dev1/mpf/config_players/queue_relay_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/random_event_player.py` & `mpf-0.80.0.dev1/mpf/config_players/random_event_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/score_queue_player.py` & `mpf-0.80.0.dev1/mpf/config_players/score_queue_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/segment_display_player.py` & `mpf-0.80.0.dev1/mpf/config_players/segment_display_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/show_player.py` & `mpf-0.80.0.dev1/mpf/config_players/show_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_players/variable_player.py` & `mpf-0.80.0.dev1/mpf/config_players/variable_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/config_spec.yaml` & `mpf-0.80.0.dev1/mpf/config_spec.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,16 @@
     hurry_up_event: single|event_handler|flipper_cancel
     end_bonus_event: single|event_handler|None
     keep_multiplier: single|template_bool|False
     bonus_entries: list|subconfig(bonus_entries)|
     rounding_value: single|int|None
     rounding_direction: single|str|up
 bonus_entries:
-    event: single|event_posted|
+    entry: single|str|
+    text: single|str|None
     score: single|template_int|
     reset_player_score_entry: single|bool|false
     player_score_entry: single|str|None
     skip_if_zero: single|bool|true
     skip_if_negative: single|bool|false
 coils:
     __valid_in__: machine
@@ -1316,57 +1317,14 @@
 playfield_transfers:
     __valid_in__: machine
     __type__: device
     ball_switch: single|machine(switches)|None
     transfer_events: event_handler|event_handler:ms|None
     eject_target: single|machine(ball_devices)|
     captures_from: single|machine(ball_devices)|
-playlist_player:
-    __valid_in__: machine, mode, show
-    __type__: config_player
-    __allow_others__:
-    action: single|enum(play,stop,advance,set_repeat)|play
-playlist_player_actions:
-    play:
-        action: ignore
-        playlist: single|str|
-        volume: single|gain|None
-        crossfade_mode: single|enum(use_track_setting,override,use_playlist_setting)|use_playlist_setting
-        crossfade_time: single|secs|None
-        shuffle: single|bool|None
-        repeat: single|bool|None
-        scope: single|enum(machine,player,use_playlist_setting)|use_playlist_setting
-        events_when_played: list|event_posted|use_playlist_setting
-        events_when_stopped: list|event_posted|use_playlist_setting
-        events_when_looping: list|event_posted|use_playlist_setting
-        events_when_sound_changed: list|event_posted|use_playlist_setting
-        events_when_sound_stopped: list|event_posted|use_playlist_setting
-    stop:
-        action: ignore
-        fade_out: single|secs|0
-    advance:
-        action: ignore
-        none: ignore
-    set_repeat:
-        action: ignore
-        repeat: single|bool|true
-playlists:
-    __valid_in__: machine, mode
-    __type__: config_dict
-    crossfade_mode: single|enum(use_track_setting,override)|use_track_setting
-    crossfade_time: single|secs|0
-    shuffle: single|bool|false
-    repeat: single|bool|false
-    scope: single|enum(machine,player)|machine
-    sounds: list|str|
-    events_when_played: list|event_posted|None
-    events_when_stopped: list|event_posted|None
-    events_when_looping: list|event_posted|None
-    events_when_sound_changed: list|event_posted|None
-    events_when_sound_stopped: list|event_posted|None
 plugins:
     __valid_in__: machine                      # todo add to validator
     __type__: list
 pololu_maestro:
     __valid_in__: machine
     __type__: config
     port: single|str|
@@ -1685,34 +1643,24 @@
 shows:
     __valid_in__: machine, mode                      # todo add to validator
     __type__: named_lists
 slide_player:
     __valid_in__: machine, mode, show
     __type__: config_player
     target: single|str|None
-    background_color: single|kivycolor|000000ff
     priority: single|int_or_token|None               # todo should this be 0?
-    show: single|bool|true
-    force: single|bool|false
     transition: ignore
     transition_out: ignore
-    widgets: ignore
     expire: single|secs|None
     slide: single|str|None
     tokens: dict|str:str|None
-    action: single|enum(play,remove)|play
-slides:
-    __valid_in__: machine, mode
-    __type__: named_lists
-    debug: single|bool|false
-    expire: single|secs|None
-    background_color: single|kivycolor|000000ff
-    opacity: single|float|1.0
-    transition_out: ignore
-    __allow_others__:
+    action: single|enum(play,remove,method,update,preload,queue,queue_first,queue_immediate)|play
+    queue: single|str|None
+    max_queue_time: single|secs|None
+    method: single|str|None
 snux:
     __valid_in__: machine
     __type__: config
     diag_led_driver: single|machine(coils)|
     console_log: single|enum(none,basic,full)|none
     file_log: single|enum(none,basic,full)|basic
 smartmatrix:
@@ -1726,156 +1674,43 @@
 smart_virtual:
     __valid_in__: machine
     __type__: config
     simulate_manual_plunger: single|bool|false
     simulate_manual_plunger_timeout: single|ms|10s
     console_log: single|enum(none,basic,full)|none
     file_log: single|enum(none,basic,full)|basic
-sound_loop_player:
-    __valid_in__: machine, mode, show
-    __type__: config_player
-    __allow_others__:
-    action: single|enum(play,stop,stop_looping,jump_to,play_layer,stop_layer,stop_looping_layer)|play
-sound_loop_player_actions:
-    play:
-        action: ignore
-        sound_loop_set: single|str|
-        volume: single|gain|None
-        fade_in: single|secs|None
-        fade_out: single|secs|None
-        start_at: single|secs|0
-        timing: single|enum(now,loop_end,next_beat_interval,next_time_interval)|loop_end
-        interval: single|float|1
-        synchronize: single|bool|false
-        events_when_played: list|event_posted|use_sound_loop_setting
-        events_when_stopped: list|event_posted|use_sound_loop_setting
-        events_when_looping: list|event_posted|use_sound_loop_setting
-        mode_end_action: single|enum(stop,stop_looping,use_sound_loop_setting)|use_sound_loop_setting
-    stop:
-        action: ignore
-        fade_out: single|secs|None
-    stop_looping:
-        action: ignore
-        none: ignore
-    jump_to:
-        action: ignore
-        time: single|secs|0
-    play_layer:
-        action: ignore
-        layer: single|int|
-        volume: single|gain|None
-        timing: single|enum(now,loop_end)|loop_end
-        fade_in: single|secs|0
-    stop_layer:
-        action: ignore
-        layer: single|int|
-        fade_out: single|secs|0
-    stop_looping_layer:
-        action: ignore
-        layer: single|int|
-sound_loop_sets:
-    __valid_in__: machine, mode
-    __type__: config_dict
-    sound: single|str|
-    volume: single|gain|None
-    tempo: single|float|60.0
-    layers:
-        sound: single|str|
-        volume: single|gain|None
-        initial_state: single|enum(play,stop)|play
-    events_when_played: list|event_posted|None
-    events_when_stopped: list|event_posted|None
-    events_when_looping: list|event_posted|None
-    fade_in: single|secs|0
-    fade_out: single|secs|0
-    mode_end_action: single|enum(stop,stop_looping)|stop
 sound_player:
     __valid_in__: machine, mode, show
     __type__: config_player
     block: single|bool|false
-    action: single|enum(play,stop,stop_looping,load,unload)|play
+    action: single|enum(play,replace,stop,stop_looping,load,unload)|play
     delay: single|secs|None
-    track: single|str|None
+    bus: single|str|None
     volume: single|gain|None
     ducking: single|subconfig(sound_ducking)|None
     pan: single|float_or_token|None
     loops: single|int_or_token|None
     priority: single|int_or_token|None
     start_at: single|secs|None
     fade_in: single|secs|None
     fade_out: single|secs|None
     about_to_finish_time: single|secs|-1
     max_queue_time: single|secs|-1
-    events_when_played: list|event_posted|use_sound_setting
-    events_when_stopped: list|event_posted|use_sound_setting
-    events_when_looping: list|event_posted|use_sound_setting
-    events_when_about_to_finish: list|event_posted|use_sound_setting
-    mode_end_action: single|enum(stop,stop_looping,use_sound_setting)|use_sound_setting
-    key: single|str|use_sound_setting
-sound_pools:
-    __valid_in__: machine, mode                      # todo add to validator
-    __type__: config_dict
-    __allow_others__:
-sound_system:
-    __valid_in__: machine
-    __type__: config
-    enabled: single|bool|true
-    buffer: single|int|2048
-    frequency: single|int|44100
-    channels: single|int|1
-    tracks: dict|str:subconfig(sound_system_tracks)|
-sound_system_tracks:
-    type: single|enum(standard,sound_loop,playlist)|standard
-    volume: single|gain|0.5
-    label: single|str|None
-    events_when_played: list|event_posted|None
-    events_when_stopped: list|event_posted|None
-    events_when_paused: list|event_posted|None
-    events_when_resumed: list|event_posted|None
-    ducking: single|subconfig(sound_ducking)|None
-    simultaneous_sounds: single|int|8       # only standard
-    max_layers: single|int|8                # only sound_loop
-    crossfade_time: single|secs|0           # only playlist
-sounds:
-    __valid_in__: machine, mode
-    __type__: config_dict
-    file: single|str|None
-    track: single|str|None
-    volume: single|gain|0.5
-    pan: single|float|0
-    streaming: single|bool|false
-    loops: single|int|0
-    loop_start_at: single|secs|0
-    loop_end_at: single|secs|None
-    priority: single|int|0
-    start_at: single|secs|0
-    fade_in: single|secs|0
-    fade_out: single|secs|0
-    about_to_finish_time: single|secs|None
-    max_queue_time: single|secs|None
-    simultaneous_limit: single|int|None
-    stealing_method: single|enum(skip,oldest,newest)|oldest
     events_when_played: list|event_posted|None
     events_when_stopped: list|event_posted|None
     events_when_looping: list|event_posted|None
     events_when_about_to_finish: list|event_posted|None
-    mode_end_action: single|enum(stop,stop_looping)|stop_looping
     key: single|str|None
-    markers: list|subconfig(sound_marker)|None
-    ducking: single|subconfig(sound_ducking)|None
 sound_ducking:
-    target: list|str|
-    delay: single|secs|0
-    attack: single|secs|10ms
-    attenuation: single|gain|1.0
-    release_point: single|secs|0
-    release: single|secs|10ms
-sound_marker:
-    time: single|secs|
-    events: list|event_posted|
+    bus: single|str|None
+    attack: single|secs|
+    attenuation: single|float|
+    delay: single|secs|0.0
+    release_point: single|secs|
+    release: single|secs|
 speedometers:
     __valid_in__: machine, mode
     __type__: device
     start_switch: single|machine(switches)|None
     stop_switch: single|machine(switches)|None
 spi_bit_bang:
     __valid_in__: machine
@@ -2064,20 +1899,14 @@
     control_events: list|subconfig(timer_control_events)|None
     restart_on_complete: single|bool|false
     bcp: single|bool|false
 timer_control_events:  # subconfig for mode timers
     action: single|enum(add,subtract,jump,start,stop,reset,restart,pause,set_tick_interval,change_tick_interval,reset_tick_interval)|
     event: single|event_handler|
     value: single|template_float|None  # float for change_tick_interval, int for the rest
-track_player:
-    __valid_in__: machine, mode, show
-    __type__: config_player
-    action: single|enum(play,stop,pause,set_volume,stop_all_sounds)|
-    volume: single|gain|None
-    fade: single|secs|0.1sec
 transitions:
     push:
         type: single|str|
         direction: single|str|left
         easing: single|str|out_quad
         duration: single|secs|1
     move_in:
@@ -2158,19 +1987,24 @@
     __valid_in__: machine
     __type__: config
     debug: single|bool|false
     listen_port: single|int|50051
 widget_player:
     __valid_in__: machine, mode, show
     __type__: config_player
+    priority: single|int_or_token|None
     slide: single|str|None
-    action: single|enum(add,remove,update)|add
+    action: single|enum(play,remove,update,preload,method)|play
+    method: ignore
     key: single|str|None
-    widget_settings: ignore
     target: single|str|None
+    expire: single|secs|None
+    tokens: dict|str:str|None
+    x: single|int|0
+    y: single|int|0
 widget_styles:
     __valid_in__: machine, mode
     __type__: config_dict
     color: single|kivycolor|ffffffff
     __allow_others__:
     # TODO: add all valid attributes
 widgets:
```

### Comparing `mpf-0.57.1.dev4/mpf/core/assets.py` & `mpf-0.80.0.dev1/mpf/core/assets.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/async_mode.py` & `mpf-0.80.0.dev1/mpf/core/async_mode.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/ball_controller.py` & `mpf-0.80.0.dev1/mpf/core/ball_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/ball_search.py` & `mpf-0.80.0.dev1/mpf/core/ball_search.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/bcp/bcp.py` & `mpf-0.80.0.dev1/mpf/core/bcp/bcp.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/bcp/bcp_client.py` & `mpf-0.80.0.dev1/mpf/core/bcp/bcp_client.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/bcp/bcp_interface.py` & `mpf-0.80.0.dev1/mpf/core/bcp/bcp_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,31 +454,35 @@
     def _monitor_machine_vars(self, client):
         # Setup machine variables to be monitored (if necessary)
         if not self.machine.bcp.transport.get_transports_for_handler("_machine_vars"):
             self.machine.variables.machine_var_monitor = True
             self.machine.register_monitor('machine_vars', self._machine_var_change)
 
         # Send initial machine variable values
-        for s in ("standard", "feature", "game", "coin"):
-            self._send_machine_vars(client, setting_type=s)
+        self._send_machine_vars(client)
+        self._send_machine_settings(client)
 
         # Establish handler for machine variable changes
         self.machine.bcp.transport.add_handler_to_transport("_machine_vars", client)
 
     def _monitor_machine_vars_stop(self, client):
         self.machine.bcp.transport.remove_transport_from_handle("_machine_vars", client)
 
         # If there are no more clients monitoring machine variables, stop monitoring
         if not self.machine.bcp.transport.get_transports_for_handler("_machine_vars"):
             self.machine.machine_var_monitor = False
 
-    def _send_machine_vars(self, client, setting_type=None):
-        self.machine.bcp.transport.send_to_client(
-            client, bcp_command='settings',
-            settings=Util.convert_to_simply_type(self.machine.settings.get_settings(setting_type)))
+    def _send_machine_settings(self, client, setting_type=None):
+        settings = [setting_type] if setting_type else ["standard", "feature", "game", "coin"]
+        for s in settings:
+            self.machine.bcp.transport.send_to_client(
+                client, bcp_command='settings',
+                settings=Util.convert_to_simply_type(self.machine.settings.get_settings(s)))
+
+    def _send_machine_vars(self, client):
         for var_name, settings in self.machine.variables.machine_vars.items():
             self.machine.bcp.transport.send_to_client(client, bcp_command='machine_variable',
                                                       name=var_name,
                                                       value=settings['value'])
 
     # pylint: disable-msg=too-many-arguments
     def _player_var_change(self, name, value, prev_value, change, player_num):
```

### Comparing `mpf-0.57.1.dev4/mpf/core/bcp/bcp_pickle_client.py` & `mpf-0.80.0.dev1/mpf/core/bcp/bcp_pickle_client.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/bcp/bcp_server.py` & `mpf-0.80.0.dev1/mpf/core/bcp/bcp_server.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/bcp/bcp_socket_client.py` & `mpf-0.80.0.dev1/mpf/core/bcp/bcp_socket_client.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/bcp/bcp_transport.py` & `mpf-0.80.0.dev1/mpf/core/bcp/bcp_transport.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/case_insensitive_dict.py` & `mpf-0.80.0.dev1/mpf/core/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/clock.py` & `mpf-0.80.0.dev1/mpf/core/clock.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/config_loader.py` & `mpf-0.80.0.dev1/mpf/core/config_loader.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/config_player.py` & `mpf-0.80.0.dev1/mpf/core/config_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/config_processor.py` & `mpf-0.80.0.dev1/mpf/core/config_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,22 +145,28 @@
                 best_similarity = similarity
 
         return best_key
 
     def _check_sections(self, config_spec, config, config_type, filename, ignore_unknown_sections):
         if not isinstance(config, dict):
             raise ConfigFileError("Config should be a dict: {}".format(config), 1, self.log.name, filename)
+
+        deprecated_080 = ["playlists", "playlist_player", "slides", "sounds", "sound_pools", "sound_loop_player",
+                          "sound_loop_sets", "sound_system", "track_player", "widgets"]
         for k in config.keys():
             if k in config_spec:
                 if config_type not in config_spec[k]['__valid_in__']:
                     raise ConfigFileError('Found a "{}:" section in config file {}, '
                                           'but that section is not valid in {} config '
                                           'files (only in {}).'.format(k, filename, config_type,
                                                                        config_spec[k]['__valid_in__']),
                                           2, self.log.name, filename)
+            elif k in deprecated_080:
+                # MPF 0.80 DEPRECATION
+                self.log.warning("Config section '%s' is deprecated in MPF 0.80 and will be ignored.", k)
             elif not ignore_unknown_sections:
                 suggestion = self._find_similar_key(k, config_spec, config_type)
 
                 raise ConfigFileError('Found a "{}:" section in config file {}, '
                                       'but that section name is unknown. Did you mean "{}:" '
                                       'instead?.'.format(k, filename, suggestion), 3, self.log.name,
                                       filename)
```

### Comparing `mpf-0.57.1.dev4/mpf/core/config_spec_loader.py` & `mpf-0.80.0.dev1/mpf/core/config_spec_loader.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/config_validator.py` & `mpf-0.80.0.dev1/mpf/core/config_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -323,14 +323,24 @@
 
                     if "mpf" in self.machine.config and self.machine.config['mpf']['allow_invalid_config_sections']:
 
                         self.log.warning('Unrecognized config setting. "%s" is '
                                          'not a valid setting name.',
                                          path_string)
 
+                    elif k == "track":
+                        # MPF 0.80 DEPRECATED
+                        self.log.error('Your config contains a value for "track" in '
+                                       'setting "%s", but "track" has been replaced '
+                                       'with "bus" in MPF 0.80.', path_string)
+
+                        raise ConfigFileError('Your config contains a value for "track" in '
+                                              'setting "' + path_string + '", but "track" has '
+                                              'been replaced with "bus" in MPF 0.80.', 2, self.log.name)
+
                     else:
                         self.log.error('Your config contains a value for the '
                                        'setting "%s", but this is not a valid '
                                        'setting name.', path_string)
 
                         raise ConfigFileError('Your config contains a value for the '
                                               'setting "' + path_string + '", but this is not a valid '
```

### Comparing `mpf-0.57.1.dev4/mpf/core/crash_reporter.py` & `mpf-0.80.0.dev1/mpf/core/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/custom_code.py` & `mpf-0.80.0.dev1/mpf/core/custom_code.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/data_manager.py` & `mpf-0.80.0.dev1/mpf/core/data_manager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/delays.py` & `mpf-0.80.0.dev1/mpf/core/delays.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/device.py` & `mpf-0.80.0.dev1/mpf/core/device.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/device_manager.py` & `mpf-0.80.0.dev1/mpf/core/device_manager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/device_monitor.py` & `mpf-0.80.0.dev1/mpf/core/device_monitor.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/enable_disable_mixin.py` & `mpf-0.80.0.dev1/mpf/core/enable_disable_mixin.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/events.py` & `mpf-0.80.0.dev1/mpf/core/events.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/file_interface.py` & `mpf-0.80.0.dev1/mpf/core/file_interface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/file_manager.py` & `mpf-0.80.0.dev1/mpf/core/file_manager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/light_controller.py` & `mpf-0.80.0.dev1/mpf/core/light_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/logging.py` & `mpf-0.80.0.dev1/mpf/core/logging.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/machine.py` & `mpf-0.80.0.dev1/mpf/core/machine.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/machine_vars.py` & `mpf-0.80.0.dev1/mpf/core/machine_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,19 @@
         desc: Version of your operating system.
         '''
         self.set_machine_var(name="platform_machine", value=platform_machine())
         '''machine_var: platform_machine
 
         desc: Architecture of your machine (32bit/64bit).
         '''
+        self.set_machine_var(name="log_file_path", value=self.machine.options.get('full_logfile_path', ""))
+        '''machine_var: log_file_path
+
+        desc: Absolute path of the file log for the current running game.
+        '''
 
     def __getitem__(self, key):
         """Allow the user to access a machine variable with []. This would be used is machine.variables["var_name"]."""
         return self.get_machine_var(key)
 
     def __setitem__(self, key, value):
         """Allow the user to set a machine variable with []. Used as machine.variables["var_name"] = value."""
```

### Comparing `mpf-0.57.1.dev4/mpf/core/mode.py` & `mpf-0.80.0.dev1/mpf/core/mode.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/mode_controller.py` & `mpf-0.80.0.dev1/mpf/core/mode_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/mode_device.py` & `mpf-0.80.0.dev1/mpf/core/mode_device.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/mpf_controller.py` & `mpf-0.80.0.dev1/mpf/core/mpf_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/placeholder_manager.py` & `mpf-0.80.0.dev1/mpf/core/placeholder_manager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/platform.py` & `mpf-0.80.0.dev1/mpf/core/platform.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/platform_batch_light_system.py` & `mpf-0.80.0.dev1/mpf/core/platform_batch_light_system.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/platform_controller.py` & `mpf-0.80.0.dev1/mpf/core/platform_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/player.py` & `mpf-0.80.0.dev1/mpf/core/player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/plugin.py` & `mpf-0.80.0.dev1/mpf/core/plugin.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/randomizer.py` & `mpf-0.80.0.dev1/mpf/core/randomizer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/rgb_color.py` & `mpf-0.80.0.dev1/mpf/core/rgb_color.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/rgba_color.py` & `mpf-0.80.0.dev1/mpf/core/rgba_color.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/segment_mappings.py` & `mpf-0.80.0.dev1/mpf/core/segment_mappings.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/service_controller.py` & `mpf-0.80.0.dev1/mpf/core/service_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/settings_controller.py` & `mpf-0.80.0.dev1/mpf/core/settings_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/show_controller.py` & `mpf-0.80.0.dev1/mpf/core/show_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/switch_controller.py` & `mpf-0.80.0.dev1/mpf/core/switch_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/text_ui.py` & `mpf-0.80.0.dev1/mpf/core/text_ui.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/core/utility_functions.py` & `mpf-0.80.0.dev1/mpf/core/utility_functions.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/accelerometer.py` & `mpf-0.80.0.dev1/mpf/devices/accelerometer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/achievement.py` & `mpf-0.80.0.dev1/mpf/devices/achievement.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/achievement_group.py` & `mpf-0.80.0.dev1/mpf/devices/achievement_group.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/autofire.py` & `mpf-0.80.0.dev1/mpf/devices/autofire.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/ball_count_handler.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/ball_count_handler.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/ball_device.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/ball_device.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/ball_device_ejector.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/ball_device_ejector.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/ball_device_state_handler.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/ball_device_state_handler.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/default_ball_search.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/default_ball_search.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/enable_coil_ejector.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/enable_coil_ejector.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/entrance_switch_counter.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/entrance_switch_counter.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/event_ejector.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/event_ejector.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/hold_coil_ejector.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/hold_coil_ejector.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/incoming_balls_handler.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/incoming_balls_handler.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/outgoing_balls_handler.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/outgoing_balls_handler.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/physical_ball_counter.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/physical_ball_counter.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/pulse_coil_ejector.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/pulse_coil_ejector.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_device/switch_counter.py` & `mpf-0.80.0.dev1/mpf/devices/ball_device/switch_counter.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_hold.py` & `mpf-0.80.0.dev1/mpf/devices/ball_hold.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_routing.py` & `mpf-0.80.0.dev1/mpf/devices/ball_routing.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/ball_save.py` & `mpf-0.80.0.dev1/mpf/devices/ball_save.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/blinkenlight.py` & `mpf-0.80.0.dev1/mpf/devices/blinkenlight.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/combo_switch.py` & `mpf-0.80.0.dev1/mpf/devices/combo_switch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/device_mixins.py` & `mpf-0.80.0.dev1/mpf/devices/device_mixins.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/digital_output.py` & `mpf-0.80.0.dev1/mpf/devices/digital_output.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/digital_score_reel.py` & `mpf-0.80.0.dev1/mpf/devices/digital_score_reel.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/diverter.py` & `mpf-0.80.0.dev1/mpf/devices/diverter.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/dmd.py` & `mpf-0.80.0.dev1/mpf/devices/dmd.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/driver.py` & `mpf-0.80.0.dev1/mpf/devices/driver.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/drop_target.py` & `mpf-0.80.0.dev1/mpf/devices/drop_target.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/dual_wound_coil.py` & `mpf-0.80.0.dev1/mpf/devices/dual_wound_coil.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/extra_ball.py` & `mpf-0.80.0.dev1/mpf/devices/extra_ball.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/extra_ball_group.py` & `mpf-0.80.0.dev1/mpf/devices/extra_ball_group.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/flipper.py` & `mpf-0.80.0.dev1/mpf/devices/flipper.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/hardware_sound_system.py` & `mpf-0.80.0.dev1/mpf/devices/hardware_sound_system.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/kickback.py` & `mpf-0.80.0.dev1/mpf/devices/kickback.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/light.py` & `mpf-0.80.0.dev1/mpf/devices/light.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/light_group.py` & `mpf-0.80.0.dev1/mpf/devices/light_group.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/logic_blocks.py` & `mpf-0.80.0.dev1/mpf/devices/logic_blocks.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/magnet.py` & `mpf-0.80.0.dev1/mpf/devices/magnet.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/motor.py` & `mpf-0.80.0.dev1/mpf/devices/motor.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/multiball.py` & `mpf-0.80.0.dev1/mpf/devices/multiball.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/multiball_lock.py` & `mpf-0.80.0.dev1/mpf/devices/multiball_lock.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/playfield.py` & `mpf-0.80.0.dev1/mpf/devices/playfield.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/playfield_transfer.py` & `mpf-0.80.0.dev1/mpf/devices/playfield_transfer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/power_supply_unit.py` & `mpf-0.80.0.dev1/mpf/devices/power_supply_unit.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/rgb_dmd.py` & `mpf-0.80.0.dev1/mpf/devices/rgb_dmd.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/score_queue.py` & `mpf-0.80.0.dev1/mpf/devices/score_queue.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/score_reel.py` & `mpf-0.80.0.dev1/mpf/devices/score_reel.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/score_reel_controller.py` & `mpf-0.80.0.dev1/mpf/devices/score_reel_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/score_reel_group.py` & `mpf-0.80.0.dev1/mpf/devices/score_reel_group.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/segment_display/segment_display.py` & `mpf-0.80.0.dev1/mpf/devices/segment_display/segment_display.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/segment_display/segment_display_text.py` & `mpf-0.80.0.dev1/mpf/devices/segment_display/segment_display_text.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/segment_display/text_stack_entry.py` & `mpf-0.80.0.dev1/mpf/devices/segment_display/text_stack_entry.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/segment_display/transition_manager.py` & `mpf-0.80.0.dev1/mpf/devices/segment_display/transition_manager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/segment_display/transitions.py` & `mpf-0.80.0.dev1/mpf/devices/segment_display/transitions.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/sequence_shot.py` & `mpf-0.80.0.dev1/mpf/devices/sequence_shot.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/servo.py` & `mpf-0.80.0.dev1/mpf/devices/servo.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/shot.py` & `mpf-0.80.0.dev1/mpf/devices/shot.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/shot_group.py` & `mpf-0.80.0.dev1/mpf/devices/shot_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         """Add device in mode."""
         super().device_loaded_in_mode(mode, player)
         self._check_for_complete()
         self.profile = self.config['shots'][0].profile
         self.rotation_pattern = deque(self.profile.config['rotation_pattern'])
         self.rotation_enabled = not self.config['enable_rotation_events']
         for shot in self.config['shots']:
-            self.machine.events.add_handler("{}_hit".format(shot.name), self._hit)
+            self.machine.events.add_handler("{}_hit".format(shot.name), self._hit, shot=shot.name)
             self.machine.events.add_handler("player_shot_{}".format(shot.name), self._check_for_complete)
 
     def device_removed_from_mode(self, mode):
         """Disable device when mode stops."""
         super().device_removed_from_mode(mode)
         self.machine.events.remove_handler(self._hit)
         self.machine.events.remove_handler(self._check_for_complete)
@@ -141,32 +141,32 @@
         self.restart()
 
     def restart(self):
         """Restart all member shots."""
         for shot in self.config['shots']:
             shot.restart()
 
-    def _hit(self, advancing, **kwargs):
+    def _hit(self, advancing, shot, **kwargs):
         """One of the member shots in this shot group was hit.
 
         Args:
         ----
             kwarg: {
                 profile: the current profile of the member shot that was hit
                 state: the current state of the member shot that was hit
                 advancing: boolean of whether the state is advancing
             }
         """
         del advancing
-        self.machine.events.post(self.name + '_hit')
+        self.machine.events.post(self.name + '_hit', shot=shot)
         '''event: (name)_hit
         desc: A member shots in the shot group called (name)
         has been hit.
         '''
-        self.machine.events.post("{}_{}_hit".format(self.name, kwargs['state']))
+        self.machine.events.post("{}_{}_hit".format(self.name, kwargs['state']), shot=shot)
         '''event: (name)_(state)_hit
         desc: A member shot with state (state) in the shot group (name)
         has been hit.
         '''
 
     @event_handler(9)
     def event_enable_rotation(self, **kwargs):
```

### Comparing `mpf-0.57.1.dev4/mpf/devices/show_queue.py` & `mpf-0.80.0.dev1/mpf/devices/show_queue.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/speedometer.py` & `mpf-0.80.0.dev1/mpf/devices/speedometer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/spinner.py` & `mpf-0.80.0.dev1/mpf/devices/spinner.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/state_machine.py` & `mpf-0.80.0.dev1/mpf/devices/state_machine.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/stepper.py` & `mpf-0.80.0.dev1/mpf/devices/stepper.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/switch.py` & `mpf-0.80.0.dev1/mpf/devices/switch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/timed_switch.py` & `mpf-0.80.0.dev1/mpf/devices/timed_switch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/devices/timer.py` & `mpf-0.80.0.dev1/mpf/devices/timer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/exceptions/base_error.py` & `mpf-0.80.0.dev1/mpf/exceptions/base_error.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/file_interfaces/pickle_interface.py` & `mpf-0.80.0.dev1/mpf/file_interfaces/pickle_interface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/file_interfaces/yaml_interface.py` & `mpf-0.80.0.dev1/mpf/file_interfaces/yaml_interface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/attract/code/attract.py` & `mpf-0.80.0.dev1/mpf/modes/attract/code/attract.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/bonus/code/bonus.py` & `mpf-0.80.0.dev1/mpf/modes/bonus/code/bonus.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,56 +87,65 @@
 
         try:
             entry = next(self.bonus_iterator)
         except StopIteration:
             self._subtotal()
             return
 
+        # Because all bonus events are 'bonus_entry' with a name arg, the
+        # following names are reserved for end-of-bonus behavior.
+        assert entry not in ["subtotal", "multiplier", "total"], "Bonus entry cannot be reserved word '%s'" % entry
+
         # Calling player.vars.get() instead of player.get() bypasses the
         # auto-fill zero and will throw if there is no player variable.
         # The fallback value of 1 is used for bonus entries that don't use
         # a player score, which are multiplied by one to get the bonus.
         hits = self.player.vars.get(entry['player_score_entry'], 1)
         score = entry['score'].evaluate([]) * hits
 
         if (not score and entry['skip_if_zero']) or (score < 0 and entry['skip_if_negative']):
             self.debug_log("Skipping bonus entry '%s' because its value is 0",
-                           entry['event'])
+                           entry['entry'])
             self._bonus_next_item()
             return
 
         # pylint: disable=superfluous-parens
         if self.settings["rounding_value"] and (r := (score % self.settings["rounding_value"])):
             self.debug_log("rounding bonus score %s remainder of %s", score, r)
             if self.settings["rounding_direction"] == "down":
                 score -= r
             else:
                 score += self.settings["rounding_value"] - r
 
         self.debug_log("Bonus Entry '%s': score: %s player_score_entry: %s=%s",
-                       entry['event'], score, entry['player_score_entry'], hits)
+                       entry['entry'], score, entry['player_score_entry'], hits)
 
         self.bonus_score += score
-        self.machine.events.post(entry['event'], score=score,
+        self.machine.events.post("bonus_entry", entry=entry['entry'],
+                                 score=score, text=entry['text'],
                                  bonus_score=self.bonus_score, hits=hits)
+        if entry.get("event"):
+            self.machine.events.post(entry['event'], score=score,
+                                     bonus_score=self.bonus_score, hits=hits)
         if entry['reset_player_score_entry']:
             self.player.vars[entry['player_score_entry']] = 0
 
         self.delay.add(name='bonus', ms=self.display_delay,
                        callback=self._bonus_next_item)
 
     def _subtotal(self):
         if self.player.vars.get("bonus_multiplier", 1) == 1:
             self.debug_log(
                 "Skipping bonus_multiplier event because the multiplier is 1.")
             self._total_bonus()
 
         else:
             self.debug_log("Bonus subtotal: %s", self.bonus_score)
-            self.machine.events.post('bonus_subtotal', score=self.bonus_score)
+            self.machine.events.post('bonus_entry', entry='subtotal',
+                                     text="Subtotal", score=self.bonus_score)
             '''event: bonus_subtotal
 
             desc: Posted by the bonus mode after all the individual bonus
             entries have been posted and processed.
 
             This event is typically posted just before the bonus multiplier
             screen, so if the bonus multiplier is 1, then this event will
@@ -149,35 +158,37 @@
             '''
             self.delay.add(name='bonus', ms=self.display_delay,
                            callback=self._do_multiplier)
 
     def _do_multiplier(self):
         multiplier = self.player.vars.get("bonus_multiplier", 1)
         self.debug_log("Bonus multiplier: %s", multiplier)
-        self.machine.events.post('bonus_multiplier', multiplier=multiplier)
+        self.machine.events.post('bonus_entry', entry='multiplier',
+                                 text="Multiplier", score=multiplier)
         '''event: bonus_multiplier
 
-        desc: Posted after "bonus_subtotal" and used to trigger the bonus
+        desc: Posted after bonus subtotal and used to trigger the bonus
         multiplier screen. If the bonus multiplier is 1, then this event is
         skipped.
 
         args:
 
-        multiplier: The numeric value of the bonus multiplier.
+        score: The numeric value of the bonus multiplier.
 
         '''
         self.bonus_score *= multiplier
         self.delay.add(name='bonus', ms=self.display_delay,
                        callback=self._total_bonus)
 
     def _total_bonus(self):
         self.player.add_with_kwargs("score", self.bonus_score,
                                     source=self.name)
         self.debug_log("Bonus Total: %s", self.bonus_score)
-        self.machine.events.post('bonus_total', score=self.bonus_score)
+        self.machine.events.post('bonus_entry', entry='total',
+                                 text="Total Bonus", score=self.bonus_score)
 
         if not self.settings['end_bonus_event']:
             self.delay.add(name='bonus', ms=self.display_delay,
                            callback=self._end_bonus)
 
     def _end_bonus(self, **kwargs):
         del kwargs
```

### Comparing `mpf-0.57.1.dev4/mpf/modes/carousel/code/carousel.py` & `mpf-0.80.0.dev1/mpf/modes/carousel/code/carousel.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,18 @@
 
     def _get_highlighted_item(self):
         return self._get_available_items()[self._highlighted_item_index]
 
     def _update_highlighted_item(self, direction):
         self.debug_log("Highlighted item: " + self._get_highlighted_item())
 
-        self.machine.events.post("{}_{}_highlighted".format(self.name, self._get_highlighted_item()),
-                                 direction=direction)
+        self.machine.events.post("item_highlighted",
+                                 carousel=self.name,
+                                 direction=direction,
+                                 item=self._get_highlighted_item())
         '''event (carousel_name)_(item)_highlighted
             desc: Player highlighted an item in a carousel. Mostly used to play shows or trigger slides.
             args:
                direction: The direction the carousel is moving. Either forwards or backwards. None on mode start.
             '''
 
     def _get_available_items(self):
```

### Comparing `mpf-0.57.1.dev4/mpf/modes/credits/code/credits.py` & `mpf-0.80.0.dev1/mpf/modes/credits/code/credits.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/credits/config/credits.yaml` & `mpf-0.80.0.dev1/mpf/modes/credits/config/credits.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/game/code/game.py` & `mpf-0.80.0.dev1/mpf/modes/game/code/game.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/high_score/code/high_score.py` & `mpf-0.80.0.dev1/mpf/modes/high_score/code/high_score.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/high_score/config/high_score.yaml` & `mpf-0.80.0.dev1/mpf/modes/high_score/config/high_score.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/high_score/images/back_arrow_7x7.png` & `mpf-0.80.0.dev1/mpf/modes/high_score/images/back_arrow_7x7.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/high_score/images/back_arrow_7x7_selected.png` & `mpf-0.80.0.dev1/mpf/modes/high_score/images/back_arrow_7x7_selected.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/high_score/images/end_11x7.png` & `mpf-0.80.0.dev1/mpf/modes/high_score/images/end_11x7.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/high_score/images/end_11x7_selected.png` & `mpf-0.80.0.dev1/mpf/modes/high_score/images/end_11x7_selected.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/match/code/match.py` & `mpf-0.80.0.dev1/mpf/modes/match/code/match.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/service/code/service.py` & `mpf-0.80.0.dev1/mpf/modes/service/code/service.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/service/config/service.yaml` & `mpf-0.80.0.dev1/mpf/modes/service/config/service.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,7 @@
         - service_power_on
     sw_power_off_active:
         - service_power_off
     sw_power_on_inactive:
         - service_power_off
     sw_power_on_active:
         - service_power_on
-
-sounds:
-  power_off:
-    track: sfx
-  switch_hit:
-    track: sfx
-
-sound_player:
-    service_power_off: power_off
-    service_switch_hit: switch_hit
```

### Comparing `mpf-0.57.1.dev4/mpf/modes/service/sounds/power_off.ogg` & `mpf-0.80.0.dev1/mpf/modes/service/sounds/power_off.ogg`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/service/sounds/switch_hit.ogg` & `mpf-0.80.0.dev1/mpf/modes/service/sounds/switch_hit.ogg`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/service_dmd/config/service_dmd.yaml` & `mpf-0.80.0.dev1/mpf/modes/service_dmd/config/service_dmd.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/service_segment_display/config/service_segment_display.yaml` & `mpf-0.80.0.dev1/mpf/modes/service_segment_display/config/service_segment_display.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/tilt/code/tilt.py` & `mpf-0.80.0.dev1/mpf/modes/tilt/code/tilt.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/modes/tilt/config/tilt.yaml` & `mpf-0.80.0.dev1/mpf/modes/tilt/config/tilt.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/mpfconfig.yaml` & `mpf-0.80.0.dev1/mpf/mpfconfig.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,20 @@
         queue_relay: mpf.config_players.queue_relay_player.QueueRelayPlayer
         flasher: mpf.config_players.flasher_player.FlasherPlayer
         light: mpf.config_players.light_player.LightPlayer
         random_event: mpf.config_players.random_event_player.RandomEventPlayer
         show: mpf.config_players.show_player.ShowPlayer
         variable: mpf.config_players.variable_player.VariablePlayer
         segment_display_player: mpf.config_players.segment_display_player.SegmentDisplayPlayer
+        slide_player: mpf.config_players.slide_player.SlidePlayer
+        sound_player: mpf.config_players.sound_player.SoundPlayer
         hardware_sound_player: mpf.config_players.hardware_sound_player.HardwareSoundPlayer
         score_queue_player: mpf.config_players.score_queue_player.ScoreQueuePlayer
         blinkenlight: mpf.config_players.blinkenlight_player.BlinkenlightPlayer
+        widget_player: mpf.config_players.widget_player.WidgetPlayer
 
     device_modules:
         coils: mpf.devices.driver.Driver
         digital_outputs: mpf.devices.digital_output.DigitalOutput
         dual_wound_coils: mpf.devices.dual_wound_coil.DualWoundCoil
         switches: mpf.devices.switch.Switch
         lights: mpf.devices.light.Light
@@ -256,47 +259,26 @@
       -  player
     events:
       -  game_started
       -  game_ended
     player:
       -  score
 
-sound_system:
-    tracks:
-        music:
-            volume: 0.5
-            simultaneous_sounds: 1
-        sfx:
-            volume: 0.5
-            simultaneous_sounds: 8
-        voice:
-            volume: 0.5
-            simultaneous_sounds: 1
-
 assets:
 #    default:
 #        load: preload
     file_shows:
         default:
             load: preload
         preload:
             load: preload
         on_demand:
             load: on_demand
         mode_start:
             load: mode_start
-    sounds:
-        default:
-             track: sfx
-        music:
-             track: music
-        sfx:
-             track: sfx
-        voice:
-             track: voice
 
 bcp:
     connections:
         local_display:
             host: localhost
             port: 5050
             type: mpf.core.bcp.bcp_socket_client.BCPClientSocket
```

### Comparing `mpf-0.57.1.dev4/mpf/parsers/event_reference_parser.py` & `mpf-0.80.0.dev1/mpf/parsers/event_reference_parser.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/parsers/special_events.py` & `mpf-0.80.0.dev1/mpf/parsers/special_events.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/base_serial_communicator.py` & `mpf-0.80.0.dev1/mpf/platforms/base_serial_communicator.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/driver_light_platform.py` & `mpf-0.80.0.dev1/mpf/platforms/driver_light_platform.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fadecandy.py` & `mpf-0.80.0.dev1/mpf/platforms/fadecandy.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/TODO.md` & `mpf-0.80.0.dev1/mpf/platforms/fast/TODO.md`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/communicators/aud.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/communicators/aud.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/communicators/base.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/communicators/base.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/communicators/dmd.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/communicators/dmd.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/communicators/emu.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/communicators/emu.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/communicators/exp.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/communicators/exp.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/communicators/net_nano.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/communicators/net_nano.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/communicators/net_neuron.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/communicators/net_neuron.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/communicators/net_retro.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/communicators/net_retro.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/communicators/rgb.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/communicators/rgb.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/communicators/seg.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/communicators/seg.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_audio.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_audio.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_defines.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_defines.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_dmd.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_dmd.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_driver.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_driver.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_exp_board.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_exp_board.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_gi.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_gi.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_io_board.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_io_board.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_led.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_led.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_light.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_light.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_port_detector.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_port_detector.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_segment_display.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_segment_display.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_servo.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_servo.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/fast/fast_switch.py` & `mpf-0.80.0.dev1/mpf/platforms/fast/fast_switch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/i2c_servo_controller.py` & `mpf-0.80.0.dev1/mpf/platforms/i2c_servo_controller.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/interfaces/dmd_platform.py` & `mpf-0.80.0.dev1/mpf/platforms/interfaces/dmd_platform.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/interfaces/driver_platform_interface.py` & `mpf-0.80.0.dev1/mpf/platforms/interfaces/driver_platform_interface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/interfaces/hardware_sound_platform_interface.py` & `mpf-0.80.0.dev1/mpf/platforms/interfaces/hardware_sound_platform_interface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/interfaces/i2c_platform_interface.py` & `mpf-0.80.0.dev1/mpf/platforms/interfaces/i2c_platform_interface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/interfaces/light_platform_interface.py` & `mpf-0.80.0.dev1/mpf/platforms/interfaces/light_platform_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 fade_ms = max_fade_ms
                 ratio = ((current_time + (max_fade_ms / 1000.0) - start_time) /
                          (target_time - start_time))
                 brightness = start_brightness + (target_brightness - start_brightness) * ratio
             else:
                 fade_ms = target_fade_ms
                 brightness = target_brightness
-            self.set_brightness_and_fade(min(1.0, max(brightness, 0.0)), max(fade_ms, 0))
+            self.set_brightness_and_fade(brightness, max(fade_ms, 0))
             if target_fade_ms <= max_fade_ms:
                 return
             await asyncio.sleep(interval)
 
     @abc.abstractmethod
     def set_brightness_and_fade(self, brightness: float, fade_ms: int) -> None:
         """Set the light to the specified brightness.
```

### Comparing `mpf-0.57.1.dev4/mpf/platforms/interfaces/segment_display_platform_interface.py` & `mpf-0.80.0.dev1/mpf/platforms/interfaces/segment_display_platform_interface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/interfaces/servo_platform_interface.py` & `mpf-0.80.0.dev1/mpf/platforms/interfaces/servo_platform_interface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/interfaces/stepper_platform_interface.py` & `mpf-0.80.0.dev1/mpf/platforms/interfaces/stepper_platform_interface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/interfaces/switch_platform_interface.py` & `mpf-0.80.0.dev1/mpf/platforms/interfaces/switch_platform_interface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/light_segment_displays.py` & `mpf-0.80.0.dev1/mpf/platforms/light_segment_displays.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/lisy/defines.py` & `mpf-0.80.0.dev1/mpf/platforms/lisy/defines.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/lisy/lisy.py` & `mpf-0.80.0.dev1/mpf/platforms/lisy/lisy.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/mma8451.py` & `mpf-0.80.0.dev1/mpf/platforms/mma8451.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/mypinballs/mypinballs.py` & `mpf-0.80.0.dev1/mpf/platforms/mypinballs/mypinballs.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/openpixel.py` & `mpf-0.80.0.dev1/mpf/platforms/openpixel.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/opp/opp.py` & `mpf-0.80.0.dev1/mpf/platforms/opp/opp.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/opp/opp_coil.py` & `mpf-0.80.0.dev1/mpf/platforms/opp/opp_coil.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/opp/opp_incand.py` & `mpf-0.80.0.dev1/mpf/platforms/opp/opp_incand.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/opp/opp_modern_lights.py` & `mpf-0.80.0.dev1/mpf/platforms/opp/opp_modern_lights.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/opp/opp_rs232_intf.py` & `mpf-0.80.0.dev1/mpf/platforms/opp/opp_rs232_intf.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/opp/opp_serial_communicator.py` & `mpf-0.80.0.dev1/mpf/platforms/opp/opp_serial_communicator.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/opp/opp_servo.py` & `mpf-0.80.0.dev1/mpf/platforms/opp/opp_servo.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/opp/opp_switch.py` & `mpf-0.80.0.dev1/mpf/platforms/opp/opp_switch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/osc.py` & `mpf-0.80.0.dev1/mpf/platforms/osc.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/p3_roc.py` & `mpf-0.80.0.dev1/mpf/platforms/p3_roc.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/p_roc.py` & `mpf-0.80.0.dev1/mpf/platforms/p_roc.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/p_roc_common.py` & `mpf-0.80.0.dev1/mpf/platforms/p_roc_common.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/p_roc_devices.py` & `mpf-0.80.0.dev1/mpf/platforms/p_roc_devices.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pin2dmd.py` & `mpf-0.80.0.dev1/mpf/platforms/pin2dmd.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pinproc/osx/pinproc.so` & `mpf-0.80.0.dev1/mpf/platforms/pinproc/osx/pinproc.so`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pkone/pkone.py` & `mpf-0.80.0.dev1/mpf/platforms/pkone/pkone.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_coil.py` & `mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_coil.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_extension.py` & `mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_extension.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_lights.py` & `mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_lights.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_lightshow.py` & `mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_lightshow.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_serial_communicator.py` & `mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_serial_communicator.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_servo.py` & `mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_servo.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pkone/pkone_switch.py` & `mpf-0.80.0.dev1/mpf/platforms/pkone/pkone_switch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pololu/pololu_tic.py` & `mpf-0.80.0.dev1/mpf/platforms/pololu/pololu_tic.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pololu/pololu_ticcmd_wrapper.py` & `mpf-0.80.0.dev1/mpf/platforms/pololu/pololu_ticcmd_wrapper.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/pololu_maestro.py` & `mpf-0.80.0.dev1/mpf/platforms/pololu_maestro.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/rpi/rpi.py` & `mpf-0.80.0.dev1/mpf/platforms/rpi/rpi.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/rpi_dmd.py` & `mpf-0.80.0.dev1/mpf/platforms/rpi_dmd.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/smart_virtual.py` & `mpf-0.80.0.dev1/mpf/platforms/smart_virtual.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/smartmatrix.py` & `mpf-0.80.0.dev1/mpf/platforms/smartmatrix.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/smbus2.py` & `mpf-0.80.0.dev1/mpf/platforms/smbus2.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/snux.py` & `mpf-0.80.0.dev1/mpf/platforms/snux.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/spi_bit_bang.py` & `mpf-0.80.0.dev1/mpf/platforms/spi_bit_bang.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/spike/spike.py` & `mpf-0.80.0.dev1/mpf/platforms/spike/spike.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/spike/spike_defines.py` & `mpf-0.80.0.dev1/mpf/platforms/spike/spike_defines.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/step_stick.py` & `mpf-0.80.0.dev1/mpf/platforms/step_stick.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/system11.py` & `mpf-0.80.0.dev1/mpf/platforms/system11.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/trinamics/TMCL.py` & `mpf-0.80.0.dev1/mpf/platforms/trinamics/TMCL.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/trinamics_steprocker.py` & `mpf-0.80.0.dev1/mpf/platforms/trinamics_steprocker.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/virtual.py` & `mpf-0.80.0.dev1/mpf/platforms/virtual.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/virtual_pinball/virtual_pinball.py` & `mpf-0.80.0.dev1/mpf/platforms/virtual_pinball/virtual_pinball.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/generate.py` & `mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/generate.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/platform_pb2.py` & `mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/platform_pb2.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/platform_pb2_grpc.py` & `mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/platform_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/protobuf/platform.proto` & `mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/protobuf/platform.proto`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/service.py` & `mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/service.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/test_client.py` & `mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/test_client.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/test_server.py` & `mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/test_server.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/platforms/visual_pinball_engine/visual_pinball_engine.py` & `mpf-0.80.0.dev1/mpf/platforms/visual_pinball_engine/visual_pinball_engine.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/plugins/auditor.py` & `mpf-0.80.0.dev1/mpf/plugins/auditor.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/plugins/info_lights.py` & `mpf-0.80.0.dev1/mpf/plugins/info_lights.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/plugins/platform_integration_test_runner.py` & `mpf-0.80.0.dev1/mpf/plugins/platform_integration_test_runner.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/plugins/switch_player.py` & `mpf-0.80.0.dev1/mpf/plugins/switch_player.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/plugins/twitch/twitch_client.py` & `mpf-0.80.0.dev1/mpf/plugins/twitch/twitch_client.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/plugins/twitch_bot.py` & `mpf-0.80.0.dev1/mpf/plugins/twitch_bot.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/plugins/virtual_segment_display_connector.py` & `mpf-0.80.0.dev1/mpf/plugins/virtual_segment_display_connector.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/MpfBcpTestCase.py` & `mpf-0.80.0.dev1/mpf/tests/MpfBcpTestCase.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/MpfDocTestCase.py` & `mpf-0.80.0.dev1/mpf/tests/MpfDocTestCase.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/MpfFakeGameTestCase.py` & `mpf-0.80.0.dev1/mpf/tests/MpfFakeGameTestCase.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/MpfGameTestCase.py` & `mpf-0.80.0.dev1/mpf/tests/MpfGameTestCase.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/MpfIntegrationDocTestCase.py` & `mpf-0.80.0.dev1/mpf/tests/MpfIntegrationDocTestCase.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/MpfMachineTestCase.py` & `mpf-0.80.0.dev1/mpf/tests/MpfMachineTestCase.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/MpfPlatformIntegrationTest.py` & `mpf-0.80.0.dev1/mpf/tests/MpfPlatformIntegrationTest.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/MpfTestCase.py` & `mpf-0.80.0.dev1/mpf/tests/MpfTestCase.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/README.md` & `mpf-0.80.0.dev1/mpf/tests/README.md`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/TestDataManager.py` & `mpf-0.80.0.dev1/mpf/tests/TestDataManager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/loop.py` & `mpf-0.80.0.dev1/mpf/tests/loop.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/auto_select/config/auto_select.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/auto_select/config/auto_select.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/achievement/modes/base/config/base.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/achievement/modes/base/config/base.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/apc/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/apc/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/config/test_asset_loading.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/config/test_asset_loading.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/custom1/show8.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/custom1/show8.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/mode_start/show9.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/mode_start/show9.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/on_demand/show10.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/on_demand/show10.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/preload/show7.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/preload/show7.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/modes/mode1/shows/show6.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/modes/mode1/shows/show6.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/custom1/show11.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/custom1/show11.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/custom1/show13.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/custom1/show13.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/on_demand/show5.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/on_demand/show5.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/preload/show4.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/preload/show4.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/preload/subfolder/show4b.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/preload/subfolder/show4b.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/show1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/show1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/show12.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/show12.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/show2.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/show2.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/asset_manager/shows/show3.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/asset_manager/shows/show3.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/autofire/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/autofire/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_controller/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_controller/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_controller/config/regression.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_controller/config/regression.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_auto_manual_plunger.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_auto_manual_plunger.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_event_confirmation.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_event_confirmation.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_event_ejector.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_event_ejector.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_jam_switch.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_jam_switch.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_manual_with_target.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_manual_with_target.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_no_plunger_switch.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_no_plunger_switch.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_routing.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_routing.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_switch_confirmation.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_switch_confirmation.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_ball_device_trigger_events.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_ball_device_trigger_events.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_gottlieb_trough.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_gottlieb_trough.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_hold_coil.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_hold_coil.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_jam_and_ball_left.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_jam_and_ball_left.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_modern_trough_plunger_setup.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_modern_trough_plunger_setup.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_player_controlled_eject.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_player_controlled_eject.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_system_11_trough.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_system_11_trough.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/test_too_long_exit_count_delay.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/test_too_long_exit_count_delay.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_device/config/trough_entrance_switch.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_device/config/trough_entrance_switch.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_holds/config/test_ball_holds.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_holds/config/test_ball_holds.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_routing/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_routing/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_routing/modes/mode1/config/mode1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_routing/modes/mode1/config/mode1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_save/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_save/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/config/mechanical_eject.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/config/mechanical_eject.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/ball_search/config/no_eject.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/ball_search/config/no_eject.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/bcp/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/bcp/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/modes/mode1/config/mode1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/modes/mode1/config/mode1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/blinkenlight/modes/mode2/config/mode2.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/blinkenlight/modes/mode2/config/mode2.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/bonus/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/bonus/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/coil_player/config/coil_player.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/coil_player/config/coil_player.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/combo_switches/config/combo_switches.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/combo_switches/config/combo_switches.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/counters/modes/mode1/config/mode1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/counters/modes/mode1/config/mode1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/credits/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/credits/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/credits/config/config_credit_tiers.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/credits/config/config_credit_tiers.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/credits/config/config_freeplay.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/credits/config/config_freeplay.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/device/config/coils.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/device/config/coils.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/device/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/device/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/digital_score_reels/config/test_digital_score_reels.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/digital_score_reels/config/test_digital_score_reels.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/only_events_no_coils.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/only_events_no_coils.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_activation_switch_and_eject_confirm_switch.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_activation_switch_and_eject_confirm_switch.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_eject_to_oposide_sides.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_eject_to_oposide_sides.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/diverter/config/test_eject_to_oposide_sides2.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/diverter/config/test_eject_to_oposide_sides2.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/drop_targets/config/test_drop_targets.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/drop_targets/config/test_drop_targets.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/event_manager/modes/test_mode/config/test_mode.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/event_manager/modes/test_mode/config/test_mode.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/config/test_event_player.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/config/test_event_player.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/event_players/config/test_random_event_player.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/event_players/config/test_random_event_player.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/extra_ball/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/extra_ball/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/extra_ball/modes/mode1/config/mode1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/extra_ball/modes/mode1/config/mode1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/audio.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/audio.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/audio2.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/audio2.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/exp.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/exp.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/nano.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/nano.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/neuron.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/neuron.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/fast/config/retro.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/fast/config/retro.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/flippers/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/flippers/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/flippers/config/hold_no_eos.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/flippers/config/hold_no_eos.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/flippers/config/software_eos_repulse.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/flippers/config/software_eos_repulse.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/game/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/game/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/head2head/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/head2head/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/info_lights/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/info_lights/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/light/config/light.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/light/config/light.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/light/config/light_groups.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/light/config/light_groups.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/light_player/config/light_player.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/light_player/config/light_player.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/light_segment_displays/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/light_segment_displays/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/light_segment_displays/config/config_dots.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/light_segment_displays/config/config_dots.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/lisy/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/lisy/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/lisy/config/config_modern.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/lisy/config/config_modern.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/lisy/config/config_system11.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/lisy/config/config_system11.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode1/config/mode1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode1/config/mode1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode2/config/mode2.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode2/config/mode2.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode3/config/mode3.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode3/config/mode3.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/logic_blocks/modes/mode4/config/mode4.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/logic_blocks/modes/mode4/config/mode4.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/magnet/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/magnet/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/motor/config/ghostbusters.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/motor/config/ghostbusters.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/motor/config/multiposition_motor.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/motor/config/multiposition_motor.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/motor/config/multiposition_motor_home_in_the_middle.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/motor/config/multiposition_motor_home_in_the_middle.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/motor/config/multiposition_motor_start_on_end_switch.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/motor/config/multiposition_motor_start_on_end_switch.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/multiball/modes/mode1/config/mode1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/multiball/modes/mode1/config/mode1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/multiball_locks/modes/default/config/default.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/multiball_locks/modes/default/config/default.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/opp/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/opp/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/opp/config/config2.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/opp/config/config2.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/opp/config/config_stm32.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/opp/config/config_stm32.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/p3_roc/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/p3_roc/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/p_roc/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/p_roc/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/p_roc/config/snux.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/p_roc/config/snux.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/p_roc/config/wpc.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/p_roc/config/wpc.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/pkone/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/pkone/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/platform/config/test_virtual.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/platform/config/test_virtual.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/player_vars/config/player_vars.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/player_vars/config/player_vars.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/score_reels/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/score_reels/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/config/config_transition.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/config/config_transition.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/segment_display/config/game.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/segment_display/config/game.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/sequence_shot/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/sequence_shot/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/service_mode/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/service_mode/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shots/config/test_shot_groups.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shots/config/test_shot_groups.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shots/config/test_shots.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shots/config/test_shots.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base/config/base.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base/config/base.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base2/config/base2.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base2/config/base2.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/base3/config/base3.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/base3/config/base3.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode1/config/mode1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode1/config/mode1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/mode2/config/mode2.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/mode2/config/mode2.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shots/modes/rotate_with_exclude/config/rotate_with_exclude.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shots/modes/rotate_with_exclude/config/rotate_with_exclude.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shows/config/test_show_player_queue.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shows/config/test_show_player_queue.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shows/config/test_show_pools.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shows/config/test_show_pools.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shows/config/test_shows.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shows/config/test_shows.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shows/config/test_sync_ms.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shows/config/test_sync_ms.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shows/modes/mode1/config/mode1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shows/modes/mode1/config/mode1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/8linesweep.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/8linesweep.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/shows/shows/test_show1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/shows/shows/test_show1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/smart_virtual_platform/config/test_coil_fired_plunger.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/smart_virtual_platform/config/test_coil_fired_plunger.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/smart_virtual_platform/config/test_smart_virtual.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/smart_virtual_platform/config/test_smart_virtual.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/snux/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/snux/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/spi_bit_bang/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/spi_bit_bang/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/spike/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/spike/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/state_machine/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/state_machine/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/stepper/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/stepper/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/switch_player/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/switch_player/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/config/config_mechanical_eject.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/config/config_mechanical_eject.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/config/config_system_11_trough.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/config/config_system_11_trough.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/tilt/config/settings.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/tilt/config/settings.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/tilt_defaults/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/tilt_defaults/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/timer/modes/mode_with_timers/config/mode_with_timers.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/timer/modes/mode_with_timers/config/mode_with_timers.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/timer/modes/mode_with_timers2/config/mode_with_timers2.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/timer/modes/mode_with_timers2/config/mode_with_timers2.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/trinamics_steprocker/config/trinamics_steprocker.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/trinamics_steprocker/config/trinamics_steprocker.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode1/config/mode1.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode1/config/mode1.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/variable_player/modes/mode3/config/mode3.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/variable_player/modes/mode3/config/mode3.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/virtual_pinball/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/virtual_pinball/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/vpe/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/vpe/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/machine_files/vpx/config/config.yaml` & `mpf-0.80.0.dev1/mpf/tests/machine_files/vpx/config/config.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/platforms/fast.py` & `mpf-0.80.0.dev1/mpf/tests/platforms/fast.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/platforms/pinproc.py` & `mpf-0.80.0.dev1/mpf/tests/platforms/pinproc.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/regression_tests/light_player_subscriptions.yaml` & `mpf-0.80.0.dev1/mpf/tests/regression_tests/light_player_subscriptions.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/regression_tests/shot_same_show_differnent_token.yaml` & `mpf-0.80.0.dev1/mpf/tests/regression_tests/shot_same_show_differnent_token.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/regression_tests/shots_with_token_in_profile_and_shot.yaml` & `mpf-0.80.0.dev1/mpf/tests/regression_tests/shots_with_token_in_profile_and_shot.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/regression_tests/show_player_subscriptions.yaml` & `mpf-0.80.0.dev1/mpf/tests/regression_tests/show_player_subscriptions.yaml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Accelerometer.py` & `mpf-0.80.0.dev1/mpf/tests/test_Accelerometer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Achievement.py` & `mpf-0.80.0.dev1/mpf/tests/test_Achievement.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_AssetManager.py` & `mpf-0.80.0.dev1/mpf/tests/test_AssetManager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Attract.py` & `mpf-0.80.0.dev1/mpf/tests/test_Attract.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Auditor.py` & `mpf-0.80.0.dev1/mpf/tests/test_Auditor.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Autofire.py` & `mpf-0.80.0.dev1/mpf/tests/test_Autofire.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallController.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallController.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDevice.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDevice.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceAutoManualPlunger.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceAutoManualPlunger.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceEnableCoil.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceEnableCoil.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceEventEjector.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceEventEjector.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceHoldCoil.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceHoldCoil.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceJamSwitch.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceJamSwitch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceManualWithTarget.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceManualWithTarget.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceModernTroughPlungerSetup.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceModernTroughPlungerSetup.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceNoPlungerSwitch.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceNoPlungerSwitch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDevicePlayfieldLock.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDevicePlayfieldLock.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDevicePulseEject.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDevicePulseEject.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceRouting.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceRouting.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceSingle.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceSingle.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceSwitchConfirmation.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceSwitchConfirmation.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDeviceTriggerEvents.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDeviceTriggerEvents.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallDevice_SmartVirtual.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallDevice_SmartVirtual.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallHold.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallHold.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallRouting.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallRouting.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallSave.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallSave.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BallSearch.py` & `mpf-0.80.0.dev1/mpf/tests/test_BallSearch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BcpInterface.py` & `mpf-0.80.0.dev1/mpf/tests/test_BcpInterface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BcpMc.py` & `mpf-0.80.0.dev1/mpf/tests/test_BcpMc.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BcpServer.py` & `mpf-0.80.0.dev1/mpf/tests/test_BcpServer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BcpSocketClient.py` & `mpf-0.80.0.dev1/mpf/tests/test_BcpSocketClient.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Blinkenlight.py` & `mpf-0.80.0.dev1/mpf/tests/test_Blinkenlight.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_BlockingEvents.py` & `mpf-0.80.0.dev1/mpf/tests/test_BlockingEvents.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Bonus.py` & `mpf-0.80.0.dev1/mpf/tests/test_Bonus.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,19 +32,15 @@
         self.advance_time_and_run(5)
         # enter menu
         self.machine.switch_controller.process_switch("s_service_enter", state=1, logical=True)
         self.machine.switch_controller.process_switch("s_slam_tilt", state=1, logical=True)
         self.advance_time_and_run()
 
     def testBonus(self):
-        self.mock_event("bonus_ramps")
-        self.mock_event("bonus_modes")
-        self.mock_event("bonus_subtotal")
-        self.mock_event("bonus_multiplier")
-        self.mock_event("bonus_total")
+        self.mock_event("bonus_entry")
         # start game
         self._start_game()
 
         self.post_event("start_mode1")
         self.advance_time_and_run()
         self.assertTrue(self.machine.mode_controller.is_active('mode1'))
 
@@ -69,141 +65,132 @@
 
         # drain a ball
         self.machine.game.balls_in_play = 0
         self.advance_time_and_run(1)
 
         # check that bonus mode is loaded
         self.assertModeRunning('bonus')
-        self.advance_time_and_run(29)
-        self.assertEqual(3000, self._last_event_kwargs["bonus_ramps"]["score"])
-        self.assertEqual(3, self._last_event_kwargs["bonus_ramps"]["hits"])
-        self.assertEqual(10000, self._last_event_kwargs["bonus_modes"]["score"])
-        self.assertEqual(2, self._last_event_kwargs["bonus_modes"]["hits"])
-        self.assertEqual(13000, self._last_event_kwargs["bonus_subtotal"]["score"])
-        self.assertEqual(5, self._last_event_kwargs["bonus_multiplier"]["multiplier"])
-        self.assertEqual(65000, self._last_event_kwargs["bonus_total"]["score"])
+        self.advance_time_and_run(1)
+        self.assertEqual("bonus_ramps", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(3000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.assertEqual(3, self._last_event_kwargs["bonus_entry"]["hits"])
+        self.advance_time_and_run(2)
+        self.assertEqual("bonus_modes", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(10000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.assertEqual(2, self._last_event_kwargs["bonus_entry"]["hits"])
+        self.advance_time_and_run(2)
+        self.assertEqual("subtotal", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(13000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.advance_time_and_run(2)
+        self.assertEqual("multiplier", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(5, self._last_event_kwargs["bonus_entry"]["score"])
+        self.advance_time_and_run(2)
+        self.assertEqual("total", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(65000, self._last_event_kwargs["bonus_entry"]["score"])
         self.assertEqual(66337, self.machine.game.player.score)
 
         # check resets
         self.assertEqual(0, self.machine.game.player.ramps)
         self.assertEqual(2, self.machine.game.player.modes)
         self.assertEqual(5, self.machine.game.player.bonus_multiplier)
 
-        self.mock_event("bonus_ramps")
-        self.mock_event("bonus_modes")
-        self.mock_event("bonus_subtotal")
-        self.mock_event("bonus_multiplier")
-        self.mock_event("bonus_total")
+        self.advance_time_and_run(10)
+        self.mock_event("bonus_entry")
 
         # drain a ball
         self.machine.game.balls_in_play = 0
-        self.advance_time_and_run(30)
+        self.advance_time_and_run(1)
+        self.assertModeRunning('bonus')
+        self.advance_time_and_run(2)
 
-        self.assertEqual(0, self._last_event_kwargs["bonus_ramps"]["score"])
-        self.assertEqual(0, self._last_event_kwargs["bonus_ramps"]["hits"])
-        self.assertEqual(10000, self._last_event_kwargs["bonus_modes"]["score"])
-        self.assertEqual(2, self._last_event_kwargs["bonus_modes"]["hits"])
-        self.assertEqual(10000, self._last_event_kwargs["bonus_subtotal"]["score"])
-        self.assertEqual(5, self._last_event_kwargs["bonus_multiplier"]["multiplier"])
-        self.assertEqual(50000, self._last_event_kwargs["bonus_total"]["score"])
+        self.assertEqual("bonus_ramps", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(0, self._last_event_kwargs["bonus_entry"]["score"])
+        self.assertEqual(0, self._last_event_kwargs["bonus_entry"]["hits"])
+        self.advance_time_and_run(2)
+        self.assertEqual("bonus_modes", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(10000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.assertEqual(2, self._last_event_kwargs["bonus_entry"]["hits"])
+        self.advance_time_and_run(2)
+        self.assertEqual("subtotal", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(10000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.advance_time_and_run(2)
+        self.assertEqual("multiplier", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(5, self._last_event_kwargs["bonus_entry"]["score"])
+        self.advance_time_and_run(2)
+        self.assertEqual("total", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(50000, self._last_event_kwargs["bonus_entry"]["score"])
         self.assertEqual(116337, self.machine.game.player.score)
 
         # multiplier should stay the same
         self.assertEqual(0, self.machine.game.player.ramps)
         self.assertEqual(2, self.machine.game.player.modes)
         self.assertEqual(5, self.machine.game.player.bonus_multiplier)
 
         # drain a ball
         self.machine.game.balls_in_play = 0
         self.advance_time_and_run(30)
 
-        # this entry event should be in bonus even though it is 0
-        self.assertIn('bonus_ramps', self._last_event_kwargs)
-        self.assertIn('bonus_modes', self._last_event_kwargs)
-
         # make some changes for the next test
         self.machine.game.player.ramps = 1
         self.machine.game.player.bonus_multiplier = 2
 
         # test the hurry up
+        self.mock_event("bonus_entry")
         self.mock_event("bonus_start")
-        self.mock_event("bonus_ramps")
-        self.mock_event("bonus_modes")
-        self.mock_event("bonus_subtotal")
-        self.mock_event("bonus_multiplier")
-        self.mock_event("bonus_total")
 
         # drain a ball
         self.machine.game.balls_in_play = 0
         self.advance_time_and_run(1)
-
         self.assertEventCalled('bonus_start')
-        self.assertEventNotCalled('bonus_ramps')
-        self.assertEventNotCalled('bonus_modes')
-        self.assertEventNotCalled('bonus_subtotal')
-        self.assertEventNotCalled('bonus_multiplier')
-        self.assertEventNotCalled('bonus_total')
+        self.assertEventNotCalled('bonus_entry')
 
         self.advance_time_and_run(2)
-
-        self.assertEventCalled('bonus_ramps')
-        self.assertEventNotCalled('bonus_modes')
-        self.assertEventNotCalled('bonus_subtotal')
-        self.assertEventNotCalled('bonus_multiplier')
-        self.assertEventNotCalled('bonus_total')
+        self.assertEqual("bonus_ramps", self._last_event_kwargs["bonus_entry"]["entry"])
 
         self.post_event('flipper_cancel', .1)
-        self.assertEventCalled('bonus_modes')
-        self.assertEventNotCalled('bonus_subtotal')
-        self.assertEventNotCalled('bonus_multiplier')
-        self.assertEventNotCalled('bonus_total')
+        self.assertEqual("bonus_modes", self._last_event_kwargs["bonus_entry"]["entry"])
 
         self.advance_time_and_run(.5)
-        self.assertEventCalled('bonus_subtotal')
-        self.assertEventNotCalled('bonus_multiplier')
-        self.assertEventNotCalled('bonus_total')
+        self.assertEqual("subtotal", self._last_event_kwargs["bonus_entry"]["entry"])
 
         self.advance_time_and_run(.5)
-        self.assertEventCalled('bonus_multiplier')
-        self.assertEventNotCalled('bonus_total')
+        self.assertEqual("multiplier", self._last_event_kwargs["bonus_entry"]["entry"])
 
         self.advance_time_and_run(.5)
-        self.assertEventCalled('bonus_total')
+        self.assertEqual("total", self._last_event_kwargs["bonus_entry"]["entry"])
 
         # test multiplier screens are skipped if multiplier is 1
         self.advance_time_and_run(30)
         self.machine.game.player.bonus_multiplier = 1
         self.machine.game.player.ramps = 1
 
         # test the hurry up
         self.mock_event("bonus_start")
-        self.mock_event("bonus_ramps")
-        self.mock_event("bonus_modes")
-        self.mock_event("bonus_subtotal")
-        self.mock_event("bonus_multiplier")
-        self.mock_event("bonus_total")
+        self.mock_event("bonus_entry")
 
         # drain a ball
         self.machine.game.balls_in_play = 0
-        self.advance_time_and_run(30)
+        self.advance_time_and_run(3)
+
+        self.assertEqual("bonus_ramps", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(1000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.assertEqual(1, self._last_event_kwargs["bonus_entry"]["hits"])
+        self.advance_time_and_run(2)
+        self.assertEqual("bonus_modes", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(10000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.assertEqual(2, self._last_event_kwargs["bonus_entry"]["hits"])
+        self.advance_time_and_run(2)
+        self.assertEqual("total", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(11000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.assertEqual(149337, self.machine.game.player.score)
 
-        self.assertEventCalled('bonus_start')
-        self.assertEventCalled('bonus_ramps')
-        self.assertEventCalled('bonus_modes')
-        self.assertEventNotCalled('bonus_subtotal')
-        self.assertEventNotCalled('bonus_multiplier')
-        self.assertEventCalled('bonus_total')
 
     @test_config_directory("tests/machine_files/bonus_no_keep_multiplier/")
     def testBonusNoKeepMultiplier(self):
-        self.mock_event("bonus_ramps")
-        self.mock_event("bonus_modes")
-        self.mock_event("bonus_subtotal")
-        self.mock_event("bonus_multiplier")
-        self.mock_event("bonus_total")
+        self.mock_event("bonus_entry")
         # start game
         self._start_game()
 
         self.post_event("start_mode1")
         self.advance_time_and_run()
         self.assertTrue(self.machine.mode_controller.is_active('mode1'))
 
@@ -228,45 +215,51 @@
 
         # drain a ball
         self.machine.game.balls_in_play = 0
         self.advance_time_and_run(1)
 
         # check that bonus mode is loaded
         self.assertModeRunning('bonus')
-        self.advance_time_and_run(29)
-        self.assertEqual(3000, self._last_event_kwargs["bonus_ramps"]["score"])
-        self.assertEqual(3, self._last_event_kwargs["bonus_ramps"]["hits"])
-        self.assertEqual(10000, self._last_event_kwargs["bonus_modes"]["score"])
-        self.assertEqual(2, self._last_event_kwargs["bonus_modes"]["hits"])
-        self.assertEqual(13000, self._last_event_kwargs["bonus_subtotal"]["score"])
-        self.assertEqual(5, self._last_event_kwargs["bonus_multiplier"]["multiplier"])
-        self.assertEqual(65000, self._last_event_kwargs["bonus_total"]["score"])
+        self.advance_time_and_run(2)
+
+        self.assertEqual("bonus_ramps", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(3000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.assertEqual(3, self._last_event_kwargs["bonus_entry"]["hits"])
+        self.advance_time_and_run(2)
+        self.assertEqual("bonus_modes", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(10000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.assertEqual(2, self._last_event_kwargs["bonus_entry"]["hits"])
+        self.advance_time_and_run(2)
+        self.assertEqual("subtotal", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(13000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.advance_time_and_run(2)
+        self.assertEqual("multiplier", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(5, self._last_event_kwargs["bonus_entry"]["score"])
+        self.advance_time_and_run(2)
+        self.assertEqual("total", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(65000, self._last_event_kwargs["bonus_entry"]["score"])
         self.assertEqual(66337, self.machine.game.player.score)
 
         # check resets
         self.assertEqual(0, self.machine.game.player.ramps)
         self.assertEqual(2, self.machine.game.player.modes)
-        self.assertEqual(1, self.machine.game.player.bonus_multiplier)
+        self.assertEqual(5, self.machine.game.player.bonus_multiplier)
 
-        self.mock_event("bonus_ramps")
-        self.mock_event("bonus_modes")
-        self.mock_event("bonus_subtotal")
-        self.mock_event("bonus_multiplier")
-        self.mock_event("bonus_total")
+        self.mock_event("bonus_entry")
+        self.advance_time_and_run(20)
 
         # drain a ball
         self.machine.game.balls_in_play = 0
-        self.advance_time_and_run(30)
-
-        self.assertNotIn('bonus_ramps', self._last_event_kwargs)
-        self.assertEqual(10000, self._last_event_kwargs["bonus_modes"]["score"])
-        self.assertEqual(2, self._last_event_kwargs["bonus_modes"]["hits"])
-        self.assertNotIn('bonus_subtotal', self._last_event_kwargs)
-        self.assertNotIn('bonus_multiplier', self._last_event_kwargs)
-        self.assertEqual(10000, self._last_event_kwargs["bonus_total"]["score"])
+        self.advance_time_and_run(2)
+        self.assertEqual("bonus_modes", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(10000, self._last_event_kwargs["bonus_entry"]["score"])
+        self.assertEqual(2, self._last_event_kwargs["bonus_entry"]["hits"])
+        self.advance_time_and_run(2)
+        self.assertEqual("total", self._last_event_kwargs["bonus_entry"]["entry"])
+        self.assertEqual(10000, self._last_event_kwargs["bonus_entry"]["score"])
         self.assertEqual(76337, self.machine.game.player.score)
 
 
     def testBonusTilted(self):
         self.mock_event("bonus_ramps")
         self.mock_event("bonus_modes")
         self.mock_event("bonus_subtotal")
```

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Clock.py` & `mpf-0.80.0.dev1/mpf/tests/test_Clock.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_CoilPlayer.py` & `mpf-0.80.0.dev1/mpf/tests/test_CoilPlayer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ComboSwitches.py` & `mpf-0.80.0.dev1/mpf/tests/test_ComboSwitches.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_CommandCreateConfig.py` & `mpf-0.80.0.dev1/mpf/tests/test_CommandCreateConfig.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Commands.py` & `mpf-0.80.0.dev1/mpf/tests/test_Commands.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Config.py` & `mpf-0.80.0.dev1/mpf/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ConfigErrors.py` & `mpf-0.80.0.dev1/mpf/tests/test_ConfigErrors.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ConfigLoader.py` & `mpf-0.80.0.dev1/mpf/tests/test_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ConfigMissingVersion.py` & `mpf-0.80.0.dev1/mpf/tests/test_ConfigMissingVersion.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ConfigOldVersion.py` & `mpf-0.80.0.dev1/mpf/tests/test_ConfigOldVersion.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ConfigPlayers.py` & `mpf-0.80.0.dev1/mpf/tests/test_ConfigPlayers.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ConfigProcessor.py` & `mpf-0.80.0.dev1/mpf/tests/test_ConfigProcessor.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_CreditsMode.py` & `mpf-0.80.0.dev1/mpf/tests/test_CreditsMode.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DataManager.py` & `mpf-0.80.0.dev1/mpf/tests/test_DataManager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Delay.py` & `mpf-0.80.0.dev1/mpf/tests/test_Delay.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DeviceCollection.py` & `mpf-0.80.0.dev1/mpf/tests/test_DeviceCollection.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DeviceDriver.py` & `mpf-0.80.0.dev1/mpf/tests/test_DeviceDriver.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DeviceFlasher.py` & `mpf-0.80.0.dev1/mpf/tests/test_DeviceFlasher.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DeviceGI.py` & `mpf-0.80.0.dev1/mpf/tests/test_DeviceGI.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DeviceLight.py` & `mpf-0.80.0.dev1/mpf/tests/test_DeviceLight.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DeviceManager.py` & `mpf-0.80.0.dev1/mpf/tests/test_DeviceManager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DeviceMatrixLight.py` & `mpf-0.80.0.dev1/mpf/tests/test_DeviceMatrixLight.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DigitalOutput.py` & `mpf-0.80.0.dev1/mpf/tests/test_DigitalOutput.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DigitalScoreReels.py` & `mpf-0.80.0.dev1/mpf/tests/test_DigitalScoreReels.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Diverter.py` & `mpf-0.80.0.dev1/mpf/tests/test_Diverter.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Dmd.py` & `mpf-0.80.0.dev1/mpf/tests/test_Dmd.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DropTargets.py` & `mpf-0.80.0.dev1/mpf/tests/test_DropTargets.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_DualWoundCoil.py` & `mpf-0.80.0.dev1/mpf/tests/test_DualWoundCoil.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_EventManager.py` & `mpf-0.80.0.dev1/mpf/tests/test_EventManager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_EventPlayer.py` & `mpf-0.80.0.dev1/mpf/tests/test_EventPlayer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ExtraBall.py` & `mpf-0.80.0.dev1/mpf/tests/test_ExtraBall.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Fadecandy.py` & `mpf-0.80.0.dev1/mpf/tests/test_Fadecandy.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Fast.py` & `mpf-0.80.0.dev1/mpf/tests/test_Fast.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Fast_Audio.py` & `mpf-0.80.0.dev1/mpf/tests/test_Fast_Audio.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Fast_Dmd.py` & `mpf-0.80.0.dev1/mpf/tests/test_Fast_Dmd.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Fast_Exp.py` & `mpf-0.80.0.dev1/mpf/tests/test_Fast_Exp.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Fast_Nano.py` & `mpf-0.80.0.dev1/mpf/tests/test_Fast_Nano.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Fast_Neuron.py` & `mpf-0.80.0.dev1/mpf/tests/test_Fast_Neuron.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Fast_Retro.py` & `mpf-0.80.0.dev1/mpf/tests/test_Fast_Retro.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Fast_Seg.py` & `mpf-0.80.0.dev1/mpf/tests/test_Fast_Seg.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Flippers.py` & `mpf-0.80.0.dev1/mpf/tests/test_Flippers.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_FlippersHoldNoEos.py` & `mpf-0.80.0.dev1/mpf/tests/test_FlippersHoldNoEos.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_FlippersSoftwareEosRepulse.py` & `mpf-0.80.0.dev1/mpf/tests/test_FlippersSoftwareEosRepulse.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Game.py` & `mpf-0.80.0.dev1/mpf/tests/test_Game.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_GottliebTrough.py` & `mpf-0.80.0.dev1/mpf/tests/test_GottliebTrough.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Head2Head.py` & `mpf-0.80.0.dev1/mpf/tests/test_Head2Head.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_HighScoreMode.py` & `mpf-0.80.0.dev1/mpf/tests/test_HighScoreMode.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_HighScoreModeWithVars.py` & `mpf-0.80.0.dev1/mpf/tests/test_HighScoreModeWithVars.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_I2cServoController.py` & `mpf-0.80.0.dev1/mpf/tests/test_I2cServoController.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_InfoLights.py` & `mpf-0.80.0.dev1/mpf/tests/test_InfoLights.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Kickback.py` & `mpf-0.80.0.dev1/mpf/tests/test_Kickback.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_LightGroups.py` & `mpf-0.80.0.dev1/mpf/tests/test_LightGroups.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_LightPlayer.py` & `mpf-0.80.0.dev1/mpf/tests/test_LightPlayer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_LightPositions.py` & `mpf-0.80.0.dev1/mpf/tests/test_LightPositions.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_LightSegmentDisplays.py` & `mpf-0.80.0.dev1/mpf/tests/test_LightSegmentDisplays.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Lisy.py` & `mpf-0.80.0.dev1/mpf/tests/test_Lisy.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_LogicBlocks.py` & `mpf-0.80.0.dev1/mpf/tests/test_LogicBlocks.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_MMA8451.py` & `mpf-0.80.0.dev1/mpf/tests/test_MMA8451.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_MachineVariables.py` & `mpf-0.80.0.dev1/mpf/tests/test_MachineVariables.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Magnet.py` & `mpf-0.80.0.dev1/mpf/tests/test_Magnet.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_MatchMode.py` & `mpf-0.80.0.dev1/mpf/tests/test_MatchMode.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Modes.py` & `mpf-0.80.0.dev1/mpf/tests/test_Modes.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ModesConfigValidation.py` & `mpf-0.80.0.dev1/mpf/tests/test_ModesConfigValidation.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Motors.py` & `mpf-0.80.0.dev1/mpf/tests/test_Motors.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_MpfTestCase.py` & `mpf-0.80.0.dev1/mpf/tests/test_MpfTestCase.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_MultiBall.py` & `mpf-0.80.0.dev1/mpf/tests/test_MultiBall.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_MultiballLock.py` & `mpf-0.80.0.dev1/mpf/tests/test_MultiballLock.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_MyPinballs.py` & `mpf-0.80.0.dev1/mpf/tests/test_MyPinballs.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_OPP.py` & `mpf-0.80.0.dev1/mpf/tests/test_OPP.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Openpixel.py` & `mpf-0.80.0.dev1/mpf/tests/test_Openpixel.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Osc.py` & `mpf-0.80.0.dev1/mpf/tests/test_Osc.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_P3_Roc.py` & `mpf-0.80.0.dev1/mpf/tests/test_P3_Roc.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_PKONE.py` & `mpf-0.80.0.dev1/mpf/tests/test_PKONE.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_P_Roc.py` & `mpf-0.80.0.dev1/mpf/tests/test_P_Roc.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_PlaceholderManager.py` & `mpf-0.80.0.dev1/mpf/tests/test_PlaceholderManager.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Platform.py` & `mpf-0.80.0.dev1/mpf/tests/test_Platform.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_PlayerVars.py` & `mpf-0.80.0.dev1/mpf/tests/test_PlayerVars.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_PlayfieldTransfer.py` & `mpf-0.80.0.dev1/mpf/tests/test_PlayfieldTransfer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_PluginConfigPlayer.py` & `mpf-0.80.0.dev1/mpf/tests/test_PluginConfigPlayer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_PololuMaestro.py` & `mpf-0.80.0.dev1/mpf/tests/test_PololuMaestro.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_PololuTic.py` & `mpf-0.80.0.dev1/mpf/tests/test_PololuTic.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_QueueEventPlayer.py` & `mpf-0.80.0.dev1/mpf/tests/test_QueueEventPlayer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_RGBColor.py` & `mpf-0.80.0.dev1/mpf/tests/test_RGBColor.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_RandomEventPlayer.py` & `mpf-0.80.0.dev1/mpf/tests/test_RandomEventPlayer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Randomizer.py` & `mpf-0.80.0.dev1/mpf/tests/test_Randomizer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Rpi.py` & `mpf-0.80.0.dev1/mpf/tests/test_Rpi.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_RpiDmd.py` & `mpf-0.80.0.dev1/mpf/tests/test_RpiDmd.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ScoreQueue.py` & `mpf-0.80.0.dev1/mpf/tests/test_ScoreQueue.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ScoreReels.py` & `mpf-0.80.0.dev1/mpf/tests/test_ScoreReels.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_SegmentDisplay.py` & `mpf-0.80.0.dev1/mpf/tests/test_SegmentDisplay.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_SegmentMappings.py` & `mpf-0.80.0.dev1/mpf/tests/test_SegmentMappings.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_SequenceShot.py` & `mpf-0.80.0.dev1/mpf/tests/test_SequenceShot.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ServiceCli.py` & `mpf-0.80.0.dev1/mpf/tests/test_ServiceCli.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ServiceMode.py` & `mpf-0.80.0.dev1/mpf/tests/test_ServiceMode.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Servo.py` & `mpf-0.80.0.dev1/mpf/tests/test_Servo.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Settings.py` & `mpf-0.80.0.dev1/mpf/tests/test_Settings.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ShotGroups.py` & `mpf-0.80.0.dev1/mpf/tests/test_ShotGroups.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Shots.py` & `mpf-0.80.0.dev1/mpf/tests/test_Shots.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_ShowPools.py` & `mpf-0.80.0.dev1/mpf/tests/test_ShowPools.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Shows.py` & `mpf-0.80.0.dev1/mpf/tests/test_Shows.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_SmartMatrix.py` & `mpf-0.80.0.dev1/mpf/tests/test_SmartMatrix.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_SmartVirtualPlatform.py` & `mpf-0.80.0.dev1/mpf/tests/test_SmartVirtualPlatform.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Smbus2.py` & `mpf-0.80.0.dev1/mpf/tests/test_Smbus2.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Snux.py` & `mpf-0.80.0.dev1/mpf/tests/test_Snux.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_SpiBitBang.py` & `mpf-0.80.0.dev1/mpf/tests/test_SpiBitBang.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Spike.py` & `mpf-0.80.0.dev1/mpf/tests/test_Spike.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Spinners.py` & `mpf-0.80.0.dev1/mpf/tests/test_Spinners.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_StateMachine.py` & `mpf-0.80.0.dev1/mpf/tests/test_StateMachine.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_StepStick.py` & `mpf-0.80.0.dev1/mpf/tests/test_StepStick.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Stepper.py` & `mpf-0.80.0.dev1/mpf/tests/test_Stepper.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_SwitchController.py` & `mpf-0.80.0.dev1/mpf/tests/test_SwitchController.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_SwitchPlayer.py` & `mpf-0.80.0.dev1/mpf/tests/test_SwitchPlayer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_SwitchPositions.py` & `mpf-0.80.0.dev1/mpf/tests/test_SwitchPositions.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_System11Trough.py` & `mpf-0.80.0.dev1/mpf/tests/test_System11Trough.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Tilt.py` & `mpf-0.80.0.dev1/mpf/tests/test_Tilt.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_TimedSwitch.py` & `mpf-0.80.0.dev1/mpf/tests/test_TimedSwitch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Timer.py` & `mpf-0.80.0.dev1/mpf/tests/test_Timer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_TooLongExitCountDelay.py` & `mpf-0.80.0.dev1/mpf/tests/test_TooLongExitCountDelay.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_TrinamicsStepRocker.py` & `mpf-0.80.0.dev1/mpf/tests/test_TrinamicsStepRocker.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_TroughEntranceSwitch.py` & `mpf-0.80.0.dev1/mpf/tests/test_TroughEntranceSwitch.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_TwitchClient.py` & `mpf-0.80.0.dev1/mpf/tests/test_TwitchClient.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Utility_Functions.py` & `mpf-0.80.0.dev1/mpf/tests/test_Utility_Functions.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_VPX.py` & `mpf-0.80.0.dev1/mpf/tests/test_VPX.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_VariablePlayer.py` & `mpf-0.80.0.dev1/mpf/tests/test_VariablePlayer.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_Virtual.py` & `mpf-0.80.0.dev1/mpf/tests/test_Virtual.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_VirtualPinball.py` & `mpf-0.80.0.dev1/mpf/tests/test_VirtualPinball.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_VirtualSegmentDisplayConnector.py` & `mpf-0.80.0.dev1/mpf/tests/test_VirtualSegmentDisplayConnector.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_VisualPinballEngine.py` & `mpf-0.80.0.dev1/mpf/tests/test_VisualPinballEngine.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/test_YamlInterface.py` & `mpf-0.80.0.dev1/mpf/tests/test_YamlInterface.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/tests/vpe_simulator.py` & `mpf-0.80.0.dev1/mpf/tests/vpe_simulator.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/wire/base.py` & `mpf-0.80.0.dev1/mpf/wire/base.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf/wire/fast.py` & `mpf-0.80.0.dev1/mpf/wire/fast.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf-logo-200.png` & `mpf-0.80.0.dev1/mpf-logo-200.png`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/mpf.egg-info/PKG-INFO` & `mpf-0.80.0.dev1/mpf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpf
-Version: 0.57.1.dev4
+Version: 0.80.0.dev1
 Summary: The Mission Pinball Framework (MPF)
 Author-email: The Mission Pinball Framework Team <brian@missionpinball.org>
 License: MIT
 Project-URL: homepage, https://missionpinball.org
 Project-URL: support-forum, https://missionpinball.org/community/
 Keywords: pinball
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mpf-0.57.1.dev4/mpf.egg-info/SOURCES.txt` & `mpf-0.80.0.dev1/mpf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 CONTRIBUTING.md
 LICENSE.md
 Makefile
 README.md
 RELEASE.md
 get_version.py
 mpf-logo-200.png
+mpf.spec
 mypy.ini
 pyproject.toml
 setup.py
 sonar-project.properties
 test_machine.py
 test_regression.py
 .github/dependabot.yml
@@ -164,15 +165,18 @@
 mpf/config_players/plugin_player.py
 mpf/config_players/queue_event_player.py
 mpf/config_players/queue_relay_player.py
 mpf/config_players/random_event_player.py
 mpf/config_players/score_queue_player.py
 mpf/config_players/segment_display_player.py
 mpf/config_players/show_player.py
+mpf/config_players/slide_player.py
+mpf/config_players/sound_player.py
 mpf/config_players/variable_player.py
+mpf/config_players/widget_player.py
 mpf/core/__init__.py
 mpf/core/assets.py
 mpf/core/async_mode.py
 mpf/core/ball_controller.py
 mpf/core/ball_search.py
 mpf/core/case_insensitive_dict.py
 mpf/core/clock.py
```

### Comparing `mpf-0.57.1.dev4/mpf.egg-info/requires.txt` & `mpf-0.80.0.dev1/mpf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/pyproject.toml` & `mpf-0.80.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/test_machine.py` & `mpf-0.80.0.dev1/test_machine.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/test_regression.py` & `mpf-0.80.0.dev1/test_regression.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/tools/afl_fuzz.py` & `mpf-0.80.0.dev1/tools/afl_fuzz.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/tools/convert_segments.py` & `mpf-0.80.0.dev1/tools/convert_segments.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/tools/debug_run_game.py` & `mpf-0.80.0.dev1/tools/debug_run_game.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/tools/p3_switch_test.py` & `mpf-0.80.0.dev1/tools/p3_switch_test.py`

 * *Files identical despite different names*

### Comparing `mpf-0.57.1.dev4/tools/smart_matrix_dmd_teensy_code/smart_matrix_dmd_teensy_code.ino` & `mpf-0.80.0.dev1/tools/smart_matrix_dmd_teensy_code/smart_matrix_dmd_teensy_code.ino`

 * *Files identical despite different names*

