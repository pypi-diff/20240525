# Comparing `tmp/matrix_gptbot-0.3.8.tar.gz` & `tmp/matrix_gptbot-0.3.9.tar.gz`

## Comparing `matrix_gptbot-0.3.8.tar` & `matrix_gptbot-0.3.9.tar`

### file list

```diff
@@ -1,73 +1,77 @@
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/CHANGELOG.md
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/config.dist.ini
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/gptbot-pantalaimon.service
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/gptbot.service
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/pantalaimon.example.conf
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/pantalaimon_first_login.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/.forgejo/workflows/release.yml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/.vscode/launch.json
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/__init__.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/__main__.py
--rw-r--r--   0        0        0   190295 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/assets/logo.png
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/callbacks/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/callbacks/invite.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/callbacks/join.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/callbacks/message.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/callbacks/roommember.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/callbacks/sync.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/callbacks/test.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/callbacks/test_response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/classes/__init__.py
--rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/classes/bot.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/classes/dict.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/classes/logging.py
--rw-r--r--   0        0        0    25750 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/classes/openai.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/classes/trackingmore.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/classes/wolframalpha.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/botinfo.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/calculate.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/chat.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/classify.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/coin.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/custom.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/dice.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/help.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/ignoreolder.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/imagine.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/newroom.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/parcel.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/privacy.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/roomsettings.py
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/space.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/stats.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/systemmessage.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/tts.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/commands/unknown.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/migrations/__init__.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/migrations/migration_1.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/migrations/migration_2.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/migrations/migration_3.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/migrations/migration_4.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/migrations/migration_5.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/migrations/migration_6.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/migrations/migration_7.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/migrations/migration_8.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/__init__.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/base.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/datetime.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/dice.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/geocode.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/imagedescription.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/imagine.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/newroom.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/weather.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/webrequest.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/websearch.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/src/gptbot/tools/wikipedia.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/LICENSE
--rw-r--r--   0        0        0     8507 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/README.md
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/CHANGELOG.md
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/Dockerfile
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/config.dist.ini
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/docker-compose.yml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/gptbot-pantalaimon.service
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/gptbot.service
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/pantalaimon.example.conf
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/pantalaimon_first_login.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/.forgejo/workflows/docker-latest.yml
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/.forgejo/workflows/docker-tag.yml
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/.forgejo/workflows/release.yml
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/.vscode/launch.json
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/__main__.py
+-rw-r--r--   0        0        0   190295 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/assets/logo.png
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/callbacks/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/callbacks/invite.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/callbacks/join.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/callbacks/message.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/callbacks/roommember.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/callbacks/sync.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/callbacks/test.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/callbacks/test_response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/classes/__init__.py
+-rw-r--r--   0        0        0    46887 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/classes/bot.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/classes/dict.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/classes/logging.py
+-rw-r--r--   0        0        0    25692 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/classes/openai.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/classes/trackingmore.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/classes/wolframalpha.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/botinfo.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/calculate.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/chat.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/classify.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/coin.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/custom.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/dice.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/help.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/ignoreolder.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/imagine.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/newroom.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/parcel.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/privacy.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/roomsettings.py
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/space.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/stats.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/systemmessage.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/tts.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/commands/unknown.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/migrations/__init__.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/migrations/migration_1.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/migrations/migration_2.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/migrations/migration_3.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/migrations/migration_4.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/migrations/migration_5.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/migrations/migration_6.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/migrations/migration_7.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/migrations/migration_8.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/__init__.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/base.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/datetime.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/dice.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/geocode.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/imagedescription.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/imagine.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/newroom.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/weather.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/webrequest.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/websearch.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/src/gptbot/tools/wikipedia.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/LICENSE
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/README.md
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.9/PKG-INFO
```

### Comparing `matrix_gptbot-0.3.8/CHANGELOG.md` & `matrix_gptbot-0.3.9/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+### 0.3.9 (unreleased)
+
+* Add Docker support for running the bot in a container
+* Add TrackingMore dependency to pyproject.toml
+* Replace deprecated `pkg_resources` with `importlib.metadata`
+* Allow password-based login on first login
+
 ### 0.3.7 / 0.3.8 (2024-04-15)
 
 * Changes to URLs in pyproject.toml
 * Migrated build pipeline to Forgejo Actions
 
 ### 0.3.6 (2024-04-11)
```

### Comparing `matrix_gptbot-0.3.8/config.dist.ini` & `matrix_gptbot-0.3.9/config.dist.ini`

 * *Files 4% similar despite different names*

```diff
@@ -139,40 +139,41 @@
 #
 # If you are using Pantalaimon, this should be the URL of your Pantalaimon
 # instance, not the Matrix homeserver itself.
 #
 Homeserver = https://matrix.local
 
 # An Access Token for the user your bot runs as
-# Can be obtained using a request like this:
 #
 # See https://www.matrix.org/docs/guides/client-server-api#login
 # for information on how to obtain this value
 #
 AccessToken = syt_yoursynapsetoken
 
-# The Matrix user ID of the bot (@local:domain.tld)
-# Only specify this if the bot fails to figure it out by itself
+# Instead of an Access Token, you can also use a User ID and password
+# to log in. Upon first run, the bot will automatically turn this into
+# an Access Token and store it in the config file, and remove the
+# password from the config file.
+#
+# This is particularly useful if you are using Pantalaimon, where this
+# is the only (easy) way to generate an Access Token.
 #
 # UserID = @gptbot:matrix.local
+# Password = yourpassword
+
 
 ###############################################################################
 
 [Database]
 
 # Path of the main database
 # Used to "remember" settings, etc.
 #
 Path = database.db
 
-# Path of the Crypto Store - required to support encrypted rooms
-# (not tested/supported yet)
-#
-CryptoStore = store.db
-
 ###############################################################################
 
 [TrackingMore]
 
 # API key for TrackingMore
 # If not defined, the bot will not be able to provide parcel tracking
 #
```

### Comparing `matrix_gptbot-0.3.8/.forgejo/workflows/release.yml` & `matrix_gptbot-0.3.9/.forgejo/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/__main__.py` & `matrix_gptbot-0.3.9/src/gptbot/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .classes.bot import GPTBot
 
 from argparse import ArgumentParser
 from configparser import ConfigParser
 
 import signal
 import asyncio
-import pkg_resources
+import importlib.metadata
 
 def sigterm_handler(_signo, _stack_frame):
     exit()
 
 def get_version():
     try:
-        package_version = pkg_resources.get_distribution("matrix_gptbot").version
+        package_version = importlib.metadata.version("matrix_gptbot")
     except pkg_resources.DistributionNotFound:
         return None
     return package_version
 
 def main():
     # Parse command line arguments
     parser = ArgumentParser()
@@ -36,15 +36,20 @@
     args = parser.parse_args()
 
     # Read config file
     config = ConfigParser()
     config.read(args.config)
 
     # Create bot
-    bot = GPTBot.from_config(config)
+    bot, new_config = GPTBot.from_config(config)
+
+    # Update config with new values
+    if new_config:
+        with open(args.config, "w") as configfile:
+            new_config.write(configfile)
 
     # Listen for SIGTERM
     signal.signal(signal.SIGTERM, sigterm_handler)
 
     # Start bot
     try:
         asyncio.run(bot.run())
```

### Comparing `matrix_gptbot-0.3.8/src/gptbot/assets/logo.png` & `matrix_gptbot-0.3.9/src/gptbot/assets/logo.png`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/callbacks/__init__.py` & `matrix_gptbot-0.3.9/src/gptbot/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/callbacks/join.py` & `matrix_gptbot-0.3.9/src/gptbot/callbacks/join.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/callbacks/message.py` & `matrix_gptbot-0.3.9/src/gptbot/callbacks/message.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/classes/bot.py` & `matrix_gptbot-0.3.9/src/gptbot/classes/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 import traceback
 
 from .logging import Logger
 from ..migrations import migrate
 from ..callbacks import RESPONSE_CALLBACKS, EVENT_CALLBACKS
 from ..commands import COMMANDS
 from ..tools import TOOLS, Handover, StopProcessing
+
+# TODO: Make these optional based on config
 from .openai import OpenAI
 from .wolframalpha import WolframAlpha
 from .trackingmore import TrackingMore
 
 
 class GPTBot:
     # Default values
@@ -258,20 +260,30 @@
 
         # Set up the Matrix client
 
         assert "Matrix" in config, "Matrix config not found"
 
         homeserver = config["Matrix"]["Homeserver"]
         bot.matrix_client = AsyncClient(homeserver)
-        bot.matrix_client.access_token = config["Matrix"]["AccessToken"]
-        bot.matrix_client.user_id = config["Matrix"].get("UserID")
-        bot.matrix_client.device_id = config["Matrix"].get("DeviceID")
 
-        # Return the new GPTBot instance
-        return bot
+        if ("Password" in config["Matrix"]) and config.get("Matrix", "Password"):
+            await bot.matrix_client.login(password=config["Matrix"]["Password"])
+
+            config["Matrix"]["AccessToken"] = bot.matrix_client.access_token
+            config["Matrix"]["UserID"] = bot.matrix_client.user_id
+            config["Matrix"]["DeviceID"] = bot.matrix_client.device_id
+            config["Matrix"]["Password"] = ""
+
+        else:
+            bot.matrix_client.access_token = config["Matrix"]["AccessToken"]
+            bot.matrix_client.user_id = config["Matrix"].get("UserID")
+            bot.matrix_client.device_id = config["Matrix"].get("DeviceID")
+
+        # Return the new GPTBot instance and the (potentially modified) config
+        return bot, config
 
     async def _get_user_id(self) -> str:
         """Get the user ID of the bot from the whoami endpoint.
         Requires an access token to be set up.
 
         Returns:
             str: The user ID of the bot.
@@ -324,15 +336,15 @@
             try:
                 event_type = event.type
             except AttributeError:
                 try:
                     event_type = event.source["content"]["msgtype"]
                 except KeyError:
                     self.logger.log(f"Could not process event: {event}", "debug")
-                    continue # This is most likely not a message event
+                    continue  # This is most likely not a message event
 
             if event_type.startswith("gptbot"):
                 messages.append(event)
 
             elif isinstance(event, RoomMessageText):
                 if event.body.split() == ["!gptbot", "ignoreolder"]:
                     break
```

### Comparing `matrix_gptbot-0.3.8/src/gptbot/classes/logging.py` & `matrix_gptbot-0.3.9/src/gptbot/classes/logging.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/classes/openai.py` & `matrix_gptbot-0.3.9/src/gptbot/classes/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,16 +249,14 @@
                         DO NOT include any other text or syntax in your response, only the JSON object. DO NOT surround it in code tags (```). DO NOT, UNDER ANY CIRCUMSTANCES, ASK AGAIN FOR INFORMATION ALREADY PROVIDED IN THE MESSAGES YOU RECEIVED! DO NOT REQUEST MORE INFORMATION THAN ABSOLUTELY REQUIRED TO RESPOND TO THE USER'S MESSAGE! Remind the user that they may ask you to search for additional information if they need it.
                         """,
                     }
                 ]
                 + messages
             )
 
-            self.logger.log(f"{messages[0]['content']}")
-
         kwargs = {
             "model": chat_model,
             "messages": messages,
             "user": room,
         }
 
         if "gpt-3.5-turbo" in chat_model and use_tools:
```

### Comparing `matrix_gptbot-0.3.8/src/gptbot/classes/trackingmore.py` & `matrix_gptbot-0.3.9/src/gptbot/classes/trackingmore.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/classes/wolframalpha.py` & `matrix_gptbot-0.3.9/src/gptbot/classes/wolframalpha.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/__init__.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/botinfo.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/botinfo.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/calculate.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/calculate.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/classify.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/classify.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/dice.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/dice.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/help.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/help.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/imagine.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/imagine.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/newroom.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/newroom.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/parcel.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/parcel.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/privacy.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/privacy.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/roomsettings.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/roomsettings.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/space.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/space.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/stats.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/stats.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/systemmessage.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/systemmessage.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/commands/tts.py` & `matrix_gptbot-0.3.9/src/gptbot/commands/tts.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/migrations/__init__.py` & `matrix_gptbot-0.3.9/src/gptbot/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/migrations/migration_1.py` & `matrix_gptbot-0.3.9/src/gptbot/migrations/migration_1.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/migrations/migration_3.py` & `matrix_gptbot-0.3.9/src/gptbot/migrations/migration_3.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/migrations/migration_5.py` & `matrix_gptbot-0.3.9/src/gptbot/migrations/migration_5.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/migrations/migration_6.py` & `matrix_gptbot-0.3.9/src/gptbot/migrations/migration_6.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/migrations/migration_7.py` & `matrix_gptbot-0.3.9/src/gptbot/migrations/migration_7.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/migrations/migration_8.py` & `matrix_gptbot-0.3.9/src/gptbot/migrations/migration_8.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/tools/base.py` & `matrix_gptbot-0.3.9/src/gptbot/tools/base.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/tools/dice.py` & `matrix_gptbot-0.3.9/src/gptbot/tools/dice.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/tools/geocode.py` & `matrix_gptbot-0.3.9/src/gptbot/tools/geocode.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/tools/imagine.py` & `matrix_gptbot-0.3.9/src/gptbot/tools/imagine.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/tools/newroom.py` & `matrix_gptbot-0.3.9/src/gptbot/tools/newroom.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/tools/weather.py` & `matrix_gptbot-0.3.9/src/gptbot/tools/weather.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/tools/webrequest.py` & `matrix_gptbot-0.3.9/src/gptbot/tools/webrequest.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/tools/websearch.py` & `matrix_gptbot-0.3.9/src/gptbot/tools/websearch.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/src/gptbot/tools/wikipedia.py` & `matrix_gptbot-0.3.9/src/gptbot/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.8/LICENSE` & `matrix_gptbot-0.3.9/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-Copyright (c) 2023 Kumi Mitterer <gptbot@kumi.email>
+Copyright (c) 2023-2024 Kumi Mitterer <gptbot@kumi.email>, Private.coffee Team
+<support@private.coffee>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `matrix_gptbot-0.3.8/README.md` & `matrix_gptbot-0.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 [![Support Private.coffee!](https://shields.private.coffee/badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://private.coffee)
 
 GPTbot is a simple bot that uses different APIs to generate responses to
 messages in a Matrix room.
 
 ## Features
 
-- AI-generated responses to text, image and voice messages in a Matrix room 
-(chatbot)
-  - Currently supports OpenAI (`gpt-3.5-turbo` and `gpt-4`, including vision 
-  preview, `whisper` and `tts`)
+- AI-generated responses to text, image and voice messages in a Matrix room
+  (chatbot)
+  - Currently supports OpenAI (`gpt-3.5-turbo` and `gpt-4`, including vision
+    preview, `whisper` and `tts`)
   - Able to generate pictures using OpenAI `dall-e-2`/`dall-e-3` models
   - Able to browse the web to find information
-  - Able to use OpenWeatherMap to get weather information (requires separate 
-  API key)
+  - Able to use OpenWeatherMap to get weather information (requires separate
+    API key)
   - Even able to roll dice!
 - Mathematical calculations via the `!gptbot calculate` command
   - Currently supports WolframAlpha (requires separate API key)
 - Really useful commands like `!gptbot help` and `!gptbot coin`
 - sqlite3 database to store room settings
 
 ## Installation
@@ -27,15 +27,17 @@
 
 The bot has been tested with Python 3.11 on Arch, but should work with any
 current version, and should not require any special dependencies or operating
 system features.
 
 ### Production
 
-The easiest way to install the bot is to use pip to install it from pypi.
+#### PyPI
+
+The recommended way to install the bot is to use pip to install it from PyPI.
 
 ```shell
 # If desired, activate a venv first
 
 python -m venv venv
 . venv/bin/activate
 
@@ -43,17 +45,44 @@
 
 pip install matrix-gptbot[all]
 ```
 
 This will install the latest release of the bot and all required dependencies
 for all available features.
 
-You can also use `pip install git+https://git.private.coffee/kumi/matrix-gptbot.git`
+You can also use `pip install git+https://git.private.coffee/privatecoffee/matrix-gptbot.git`
 to install the latest version from the Git repository.
 
+#### Docker
+
+A `docker-compose.yml` file is provided that you can use to run the bot with
+Docker Compose. You will need to create a `config.ini` file as described in the
+`Running` section.
+
+```shell
+# Clone the repository
+git clone https://git.private.coffee/privatecoffee/matrix-gptbot.git
+cd matrix-gptbot
+
+# Create a config file
+cp config.dist.ini config.ini
+# Edit the config file to your needs
+
+# Initialize the database file
+sqlite3 database.db "SELECT 1"
+
+# Optionally, create Pantalaimon config
+cp pantalaimon.example.conf pantalaimon.conf
+# Edit the Pantalaimon config file to your needs
+# Don't forget to update config.ini to point to your Pantalaimon instance
+
+# Start the bot
+docker-compose up -d
+```
+
 #### End-to-end encryption
 
 WARNING: Using end-to-end encryption seems to sometimes cause problems with
 file attachments, especially in rooms that are not encrypted, if the same
 user also uses the bot in encrypted rooms.
 
 The bot itself does not implement end-to-end encryption. However, it can be
@@ -63,57 +92,63 @@
 To use pantalaimon, create a `pantalaimon.conf` following the example in
 `pantalaimon.example.conf`, making sure to change the homeserver URL to match
 your homeserver. Then, start pantalaimon with `pantalaimon -c pantalaimon.conf`.
 
 You first have to log in to your homeserver using `python pantalaimon_first_login.py`,
 and can then use the returned access token in your bot's `config.ini` file.
 
-Make sure to also point the bot to your pantalaimon instance by setting 
-`homeserver` to your pantalaimon instance instead of directly to your 
+Make sure to also point the bot to your pantalaimon instance by setting
+`homeserver` to your pantalaimon instance instead of directly to your
 homeserver in your `config.ini`.
 
-Note: If you don't use pantalaimon, the bot will still work, but it will not 
+Note: If you don't use pantalaimon, the bot will still work, but it will not
 be able to decrypt or encrypt messages. This means that you cannot use it in
 rooms with end-to-end encryption enabled.
 
 ### Development
 
 Clone the repository and install the requirements to a virtual environment.
 
 ```shell
 # Clone the repository
-
-git clone https://git.private.coffee/kumi/matrix-gptbot.git
+git clone https://git.private.coffee/privatecoffee/matrix-gptbot.git
 cd matrix-gptbot
 
 # If desired, activate a venv first
-
 python -m venv venv
 . venv/bin/activate
 
 # Install the bot in editable mode
-
 pip install -e .[dev]
 
 # Go to the bot directory and start working
-
 cd src/gptbot
 ```
 
 Of course, you can also fork the repository on [GitHub](https://github.com/kumitterer/matrix-gptbot/)
 and work on your own copy.
 
-### Configuration
+#### Repository policy
 
-The bot requires a configuration file to be present in the working directory.
-Copy the provided `config.dist.ini` to `config.ini` and edit it to your needs.
+Generally, the `main` branch is considered unstable and should not be used in
+production. Instead, use the latest release tag. The `main` branch is used for
+development and may contain breaking changes at any time.
+
+For development, a feature branch should be created from `main` and merged back
+into `main` with a pull request. The pull request will be reviewed and tested
+before merging.
 
 ## Running
 
-The bot can be run with `python -m gptbot`. If required, activate a venv first.
+The bot requires a configuration file to be present in the working directory.
+
+Copy the provided `config.dist.ini` to `config.ini` and edit it to your needs.
+
+The bot can then be run with `python -m gptbot`. If required, activate a venv
+first.
 
 You may want to run the bot in a screen or tmux session, or use a process
 manager like systemd. The repository contains a sample systemd service file
 (`gptbot.service`) that you can use as a starting point. You will need to
 adjust the paths in the file to match your setup, then copy it to
 `/etc/systemd/system/gptbot.service`. You can then start the bot with
 `systemctl start gptbot` and enable it to start automatically on boot with
@@ -147,26 +182,26 @@
 The bot has a selection of tools at its disposal that it will automatically use
 to generate responses. For example, if you send a message like "Draw me a
 picture of a cat", the bot will automatically use DALL-E to generate an image
 of a cat.
 
 Note that this only works if the bot is configured to use a model that supports
 tools. This currently is only the case for OpenAI's `gpt-3.5-turbo` model. If
-you wish to use `gpt-4` instead, you can set the `ForceTools` option in the 
+you wish to use `gpt-4` instead, you can set the `ForceTools` option in the
 `[OpenAI]` section of the config file to `1`. This will cause the bot to use
 `gpt-3.5-turbo` for tool generation and `gpt-4` for generating the final text
 response.
 
-Similarly, it will attempt to use the `gpt-4-vision-preview` model to "read" 
+Similarly, it will attempt to use the `gpt-4-vision-preview` model to "read"
 the contents of images if a non-vision model is used.
 
 ### Commands
 
 There are a few commands that you can use to explicitly call a certain feature
-of the bot. For example, if you want to generate an image from a text prompt, 
+of the bot. For example, if you want to generate an image from a text prompt,
 you can use the `!gptbot imagine` command. For example, `!gptbot imagine a cat`
 will cause the bot to generate an image of a cat.
 
 To learn more about the available commands, `!gptbot help` will print a list of
 available commands.
 
 ### Voice input and output
```

### Comparing `matrix_gptbot-0.3.8/pyproject.toml` & `matrix_gptbot-0.3.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "matrix-gptbot"
-version = "0.3.8"
+version = "0.3.9"
 
 authors = [
   { name="Kumi Mitterer", email="gptbot@kumi.email" },
+  { name="Private.coffee Team", email="support@private.coffee" },
 ]
 
 description = "Multifunctional Chatbot for Matrix"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
 
@@ -46,31 +47,35 @@
     "wolframalpha",
 ]
 
 e2ee = [
     "pantalaimon>=0.10.5",
 ]
 
+trackingmore = [
+    "trackingmore-api-tool",
+]
+
 all = [
-  "matrix-gptbot[openai,wolframalpha,e2ee]",
+  "matrix-gptbot[openai,wolframalpha,e2ee,trackingmore]",
   "geopy",
   "beautifulsoup4",
 ]
 
 dev = [
   "matrix-gptbot[all]",
   "black",
   "hatchling",
   "twine",
   "build",
 ]
 
 [project.urls]
-"Homepage" = "https://git.private.coffee/kumi/matrix-gptbot"
-"Bug Tracker" = "https://git.private.coffee/kumi/matrix-gptbot/issues"
-"Source Code" = "https://git.private.coffee/kumi/matrix-gptbot"
+"Homepage" = "https://git.private.coffee/privatecoffee/matrix-gptbot"
+"Bug Tracker" = "https://git.private.coffee/privatecoffee/matrix-gptbot/issues"
+"Source Code" = "https://git.private.coffee/privatecoffee/matrix-gptbot"
 
 [project.scripts]
 gptbot = "gptbot.__main__:main"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/gptbot"]
```

### Comparing `matrix_gptbot-0.3.8/PKG-INFO` & `matrix_gptbot-0.3.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.3
 Name: matrix-gptbot
-Version: 0.3.8
+Version: 0.3.9
 Summary: Multifunctional Chatbot for Matrix
-Project-URL: Homepage, https://git.private.coffee/kumi/matrix-gptbot
-Project-URL: Bug Tracker, https://git.private.coffee/kumi/matrix-gptbot/issues
-Project-URL: Source Code, https://git.private.coffee/kumi/matrix-gptbot
-Author-email: Kumi Mitterer <gptbot@kumi.email>
-License: Copyright (c) 2023 Kumi Mitterer <gptbot@kumi.email>
+Project-URL: Homepage, https://git.private.coffee/privatecoffee/matrix-gptbot
+Project-URL: Bug Tracker, https://git.private.coffee/privatecoffee/matrix-gptbot/issues
+Project-URL: Source Code, https://git.private.coffee/privatecoffee/matrix-gptbot
+Author-email: Kumi Mitterer <gptbot@kumi.email>, "Private.coffee Team" <support@private.coffee>
+License: Copyright (c) 2023-2024 Kumi Mitterer <gptbot@kumi.email>, Private.coffee Team
+        <support@private.coffee>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -37,52 +38,56 @@
 Requires-Dist: tiktoken
 Provides-Extra: all
 Requires-Dist: beautifulsoup4; extra == 'all'
 Requires-Dist: geopy; extra == 'all'
 Requires-Dist: openai>=1.2; extra == 'all'
 Requires-Dist: pantalaimon>=0.10.5; extra == 'all'
 Requires-Dist: pydub; extra == 'all'
+Requires-Dist: trackingmore-api-tool; extra == 'all'
 Requires-Dist: wolframalpha; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: beautifulsoup4; extra == 'dev'
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: geopy; extra == 'dev'
 Requires-Dist: hatchling; extra == 'dev'
 Requires-Dist: openai>=1.2; extra == 'dev'
 Requires-Dist: pantalaimon>=0.10.5; extra == 'dev'
 Requires-Dist: pydub; extra == 'dev'
+Requires-Dist: trackingmore-api-tool; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Requires-Dist: wolframalpha; extra == 'dev'
 Provides-Extra: e2ee
 Requires-Dist: pantalaimon>=0.10.5; extra == 'e2ee'
 Provides-Extra: openai
 Requires-Dist: openai>=1.2; extra == 'openai'
 Requires-Dist: pydub; extra == 'openai'
+Provides-Extra: trackingmore
+Requires-Dist: trackingmore-api-tool; extra == 'trackingmore'
 Provides-Extra: wolframalpha
 Requires-Dist: wolframalpha; extra == 'wolframalpha'
 Description-Content-Type: text/markdown
 
 # GPTbot
 
 [![Support Private.coffee!](https://shields.private.coffee/badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://private.coffee)
 
 GPTbot is a simple bot that uses different APIs to generate responses to
 messages in a Matrix room.
 
 ## Features
 
-- AI-generated responses to text, image and voice messages in a Matrix room 
-(chatbot)
-  - Currently supports OpenAI (`gpt-3.5-turbo` and `gpt-4`, including vision 
-  preview, `whisper` and `tts`)
+- AI-generated responses to text, image and voice messages in a Matrix room
+  (chatbot)
+  - Currently supports OpenAI (`gpt-3.5-turbo` and `gpt-4`, including vision
+    preview, `whisper` and `tts`)
   - Able to generate pictures using OpenAI `dall-e-2`/`dall-e-3` models
   - Able to browse the web to find information
-  - Able to use OpenWeatherMap to get weather information (requires separate 
-  API key)
+  - Able to use OpenWeatherMap to get weather information (requires separate
+    API key)
   - Even able to roll dice!
 - Mathematical calculations via the `!gptbot calculate` command
   - Currently supports WolframAlpha (requires separate API key)
 - Really useful commands like `!gptbot help` and `!gptbot coin`
 - sqlite3 database to store room settings
 
 ## Installation
@@ -91,15 +96,17 @@
 
 The bot has been tested with Python 3.11 on Arch, but should work with any
 current version, and should not require any special dependencies or operating
 system features.
 
 ### Production
 
-The easiest way to install the bot is to use pip to install it from pypi.
+#### PyPI
+
+The recommended way to install the bot is to use pip to install it from PyPI.
 
 ```shell
 # If desired, activate a venv first
 
 python -m venv venv
 . venv/bin/activate
 
@@ -107,17 +114,44 @@
 
 pip install matrix-gptbot[all]
 ```
 
 This will install the latest release of the bot and all required dependencies
 for all available features.
 
-You can also use `pip install git+https://git.private.coffee/kumi/matrix-gptbot.git`
+You can also use `pip install git+https://git.private.coffee/privatecoffee/matrix-gptbot.git`
 to install the latest version from the Git repository.
 
+#### Docker
+
+A `docker-compose.yml` file is provided that you can use to run the bot with
+Docker Compose. You will need to create a `config.ini` file as described in the
+`Running` section.
+
+```shell
+# Clone the repository
+git clone https://git.private.coffee/privatecoffee/matrix-gptbot.git
+cd matrix-gptbot
+
+# Create a config file
+cp config.dist.ini config.ini
+# Edit the config file to your needs
+
+# Initialize the database file
+sqlite3 database.db "SELECT 1"
+
+# Optionally, create Pantalaimon config
+cp pantalaimon.example.conf pantalaimon.conf
+# Edit the Pantalaimon config file to your needs
+# Don't forget to update config.ini to point to your Pantalaimon instance
+
+# Start the bot
+docker-compose up -d
+```
+
 #### End-to-end encryption
 
 WARNING: Using end-to-end encryption seems to sometimes cause problems with
 file attachments, especially in rooms that are not encrypted, if the same
 user also uses the bot in encrypted rooms.
 
 The bot itself does not implement end-to-end encryption. However, it can be
@@ -127,57 +161,63 @@
 To use pantalaimon, create a `pantalaimon.conf` following the example in
 `pantalaimon.example.conf`, making sure to change the homeserver URL to match
 your homeserver. Then, start pantalaimon with `pantalaimon -c pantalaimon.conf`.
 
 You first have to log in to your homeserver using `python pantalaimon_first_login.py`,
 and can then use the returned access token in your bot's `config.ini` file.
 
-Make sure to also point the bot to your pantalaimon instance by setting 
-`homeserver` to your pantalaimon instance instead of directly to your 
+Make sure to also point the bot to your pantalaimon instance by setting
+`homeserver` to your pantalaimon instance instead of directly to your
 homeserver in your `config.ini`.
 
-Note: If you don't use pantalaimon, the bot will still work, but it will not 
+Note: If you don't use pantalaimon, the bot will still work, but it will not
 be able to decrypt or encrypt messages. This means that you cannot use it in
 rooms with end-to-end encryption enabled.
 
 ### Development
 
 Clone the repository and install the requirements to a virtual environment.
 
 ```shell
 # Clone the repository
-
-git clone https://git.private.coffee/kumi/matrix-gptbot.git
+git clone https://git.private.coffee/privatecoffee/matrix-gptbot.git
 cd matrix-gptbot
 
 # If desired, activate a venv first
-
 python -m venv venv
 . venv/bin/activate
 
 # Install the bot in editable mode
-
 pip install -e .[dev]
 
 # Go to the bot directory and start working
-
 cd src/gptbot
 ```
 
 Of course, you can also fork the repository on [GitHub](https://github.com/kumitterer/matrix-gptbot/)
 and work on your own copy.
 
-### Configuration
+#### Repository policy
 
-The bot requires a configuration file to be present in the working directory.
-Copy the provided `config.dist.ini` to `config.ini` and edit it to your needs.
+Generally, the `main` branch is considered unstable and should not be used in
+production. Instead, use the latest release tag. The `main` branch is used for
+development and may contain breaking changes at any time.
+
+For development, a feature branch should be created from `main` and merged back
+into `main` with a pull request. The pull request will be reviewed and tested
+before merging.
 
 ## Running
 
-The bot can be run with `python -m gptbot`. If required, activate a venv first.
+The bot requires a configuration file to be present in the working directory.
+
+Copy the provided `config.dist.ini` to `config.ini` and edit it to your needs.
+
+The bot can then be run with `python -m gptbot`. If required, activate a venv
+first.
 
 You may want to run the bot in a screen or tmux session, or use a process
 manager like systemd. The repository contains a sample systemd service file
 (`gptbot.service`) that you can use as a starting point. You will need to
 adjust the paths in the file to match your setup, then copy it to
 `/etc/systemd/system/gptbot.service`. You can then start the bot with
 `systemctl start gptbot` and enable it to start automatically on boot with
@@ -211,26 +251,26 @@
 The bot has a selection of tools at its disposal that it will automatically use
 to generate responses. For example, if you send a message like "Draw me a
 picture of a cat", the bot will automatically use DALL-E to generate an image
 of a cat.
 
 Note that this only works if the bot is configured to use a model that supports
 tools. This currently is only the case for OpenAI's `gpt-3.5-turbo` model. If
-you wish to use `gpt-4` instead, you can set the `ForceTools` option in the 
+you wish to use `gpt-4` instead, you can set the `ForceTools` option in the
 `[OpenAI]` section of the config file to `1`. This will cause the bot to use
 `gpt-3.5-turbo` for tool generation and `gpt-4` for generating the final text
 response.
 
-Similarly, it will attempt to use the `gpt-4-vision-preview` model to "read" 
+Similarly, it will attempt to use the `gpt-4-vision-preview` model to "read"
 the contents of images if a non-vision model is used.
 
 ### Commands
 
 There are a few commands that you can use to explicitly call a certain feature
-of the bot. For example, if you want to generate an image from a text prompt, 
+of the bot. For example, if you want to generate an image from a text prompt,
 you can use the `!gptbot imagine` command. For example, `!gptbot imagine a cat`
 will cause the bot to generate an image of a cat.
 
 To learn more about the available commands, `!gptbot help` will print a list of
 available commands.
 
 ### Voice input and output
```

