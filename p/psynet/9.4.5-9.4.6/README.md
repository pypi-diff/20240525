# Comparing `tmp/psynet-9.4.5.tar.gz` & `tmp/psynet-9.4.6.tar.gz`

## Comparing `psynet-9.4.5.tar` & `psynet-9.4.6.tar`

### file list

```diff
@@ -1,132 +1,134 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 psynet-9.4.5/.flake8
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 psynet-9.4.5/.git-blame-ignore-revs.txt
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 psynet-9.4.5/.gitlab-ci.yml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 psynet-9.4.5/.jshintrc
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 psynet-9.4.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 psynet-9.4.5/.pylintrc
--rw-r--r--   0        0        0    49767 2020-02-02 00:00:00.000000 psynet-9.4.5/CHANGELOG.md
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 psynet-9.4.5/MANIFEST.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 psynet-9.4.5/pytest.ini
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 psynet-9.4.5/unity_interface_description.md
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/VERSION
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/__init__.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/audio_mixer.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/bot.py
--rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/command_line.py
--rw-r--r--   0        0        0    20168 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/consent.py
--rw-r--r--   0        0        0    18337 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/data.py
--rwxr-xr-x   0        0        0    48778 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/experiment.py
--rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/field.py
--rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/graphics.py
--rw-r--r--   0        0        0    16703 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/js_synth.py
--rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/lucid.py
--rw-r--r--   0        0        0    10805 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/media.py
--rw-r--r--   0        0        0    73963 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/modular_page.py
--rw-r--r--   0        0        0    31849 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/page.py
--rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/participant.py
--rw-r--r--   0        0        0    68055 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/prescreen.py
--rw-r--r--   0        0        0    11509 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/recruiters.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/test.py
--rw-r--r--   0        0        0    78194 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/timeline.py
--rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/definitions/__init__.py
--rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/definitions/gold-msi.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/demography/__init__.py
--rw-r--r--   0        0        0    37278 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/demography/general.py
--rw-r--r--   0        0        0    22781 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/demography/gmsi.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/demography/pei.py
--rw-r--r--   0        0        0    73790 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/favicon.ico
--rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/logo.png
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/logo.svg
--rw-r--r--   0        0        0    18335 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/logo_image_only.png
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/css/consent.css
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/css/dashboard_timeline.css
--rw-r--r--   0        0        0    38441 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/images/princeton-consent.png
--rw-r--r--   0        0        0    18658 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/images/unity_logo.png
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/Tonejs/LICENSE.md
--rw-r--r--   0        0        0   349554 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/Tonejs/Tone.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery/jquery-3.6.0.min.js
--rwxr-xr-x   0        0        0       10 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/.gitignore
--rwxr-xr-x   0        0        0     1082 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/LICENSE
--rwxr-xr-x   0        0        0     3099 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/README.md
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/bower.json
--rwxr-xr-x   0        0        0    27045 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/excanvas.js
--rwxr-xr-x   0        0        0    13014 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/index.html
--rwxr-xr-x   0        0        0      984 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/knob.jquery.json
--rwxr-xr-x   0        0        0      589 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/package.json
--rwxr-xr-x   0        0        0    33487 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/secretplan.jpg
--rwxr-xr-x   0        0        0    26225 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/js/jquery.knob.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/js-synthesizer/.gitignore
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/js-synthesizer/README.txt
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/js-synthesizer/demo.html
--rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/js-synthesizer/instruments.js
--rw-r--r--   0        0        0    11184 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/js-synthesizer/synthesis.js
--rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/platform-1.3.6/platform.min.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/.eslintrc.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/.gitignore
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/README.md
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/license.txt
--rw-r--r--   0        0        0    93167 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/raphael.min.js
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/scripts/dashboard_timeline.js
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/scripts/prepare_docker_image.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/abort_not_possible.html
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/abort_possible.html
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/ad.html
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consent.html
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/dashboard_timeline.html
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/exit_recruiter_lucid.html
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/final-page-bonuses.html
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/final-page-rejected-consent.html
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/final-page-successful.html
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/final-page-unsuccessful.html
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/info-page.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros.html
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/mturk_error.html
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/participant.html
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/psynet_layout.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/questions.html
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/resume.html
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/start.html
--rw-r--r--   0        0        0    67246 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/timeline-page.html
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/unity-debug-page.html
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/unity-page.html
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/wait-page.html
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/audiovisual_consent.html
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/cap-recruiter_audiovisual_consent.html
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/cap-recruiter_standard_consent.html
--rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/database_consent.html
--rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/main_consent.html
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/mturk_audiovisual_consent.html
--rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/mturk_standard_consent.html
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/open_science_consent.html
--rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/princeton_cap_recruiter_consent.html
--rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/princeton_consent.html
--rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/voluntary_with_no_compensation_consent.html
--rw-r--r--   0        0        0    62854 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control.html
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/graphics.html
--rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/prompt.html
--rw-r--r--   0        0        0   194322 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control/RecordRTC.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control/__init__.py
--rw-r--r--   0        0        0   199443 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control/adapter.js
--rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control/audio_meter.js
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control/recorder.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/__init__.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/audio.py
--rw-r--r--   0        0        0    15679 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/audio_gibbs.py
--rw-r--r--   0        0        0    52506 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/chain.py
--rw-r--r--   0        0        0    30793 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/dense.py
--rw-r--r--   0        0        0    12498 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/gibbs.py
--rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/graph.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/imitation_chain.py
--rw-r--r--   0        0        0    88618 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/main.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/mcmcp.py
--rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/record.py
--rw-r--r--   0        0        0    57654 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/static.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/video.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 psynet-9.4.5/.gitignore
--rwxr-xr-x   0        0        0     1126 2020-02-02 00:00:00.000000 psynet-9.4.5/LICENSE
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 psynet-9.4.5/README.md
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 psynet-9.4.5/pyproject.toml
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 psynet-9.4.5/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 psynet-9.4.6/.flake8
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 psynet-9.4.6/.git-blame-ignore-revs.txt
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 psynet-9.4.6/.gitlab-ci.yml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 psynet-9.4.6/.jshintrc
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 psynet-9.4.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 psynet-9.4.6/.pylintrc
+-rw-r--r--   0        0        0    50148 2020-02-02 00:00:00.000000 psynet-9.4.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 psynet-9.4.6/MANIFEST.in
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 psynet-9.4.6/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.6/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 psynet-9.4.6/pytest.ini
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 psynet-9.4.6/requirements.txt
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 psynet-9.4.6/unity_interface_description.md
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/VERSION
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/__init__.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/audio_mixer.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/bot.py
+-rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/command_line.py
+-rw-r--r--   0        0        0    20168 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/consent.py
+-rw-r--r--   0        0        0    18337 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/data.py
+-rwxr-xr-x   0        0        0    48768 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/experiment.py
+-rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/field.py
+-rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/graphics.py
+-rw-r--r--   0        0        0    16703 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/js_synth.py
+-rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/lucid.py
+-rw-r--r--   0        0        0    10805 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/media.py
+-rw-r--r--   0        0        0    73963 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/modular_page.py
+-rw-r--r--   0        0        0    31849 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/page.py
+-rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/participant.py
+-rw-r--r--   0        0        0    68055 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/prescreen.py
+-rw-r--r--   0        0        0    11509 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/recruiters.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/test.py
+-rw-r--r--   0        0        0    78194 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/timeline.py
+-rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/definitions/__init__.py
+-rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/definitions/gold-msi.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/demography/__init__.py
+-rw-r--r--   0        0        0    37278 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/demography/general.py
+-rw-r--r--   0        0        0    22781 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/demography/gmsi.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/demography/pei.py
+-rw-r--r--   0        0        0    73790 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/favicon.ico
+-rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/logo.png
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/logo.svg
+-rw-r--r--   0        0        0    18335 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/logo_image_only.png
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/css/consent.css
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/css/dashboard_timeline.css
+-rw-r--r--   0        0        0    38441 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/images/princeton-consent.png
+-rw-r--r--   0        0        0    18658 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/images/unity_logo.png
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/Tonejs/LICENSE.md
+-rw-r--r--   0        0        0   349554 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/Tonejs/Tone.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery/jquery-3.6.0.min.js
+-rwxr-xr-x   0        0        0       10 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/.gitignore
+-rwxr-xr-x   0        0        0     1082 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/LICENSE
+-rwxr-xr-x   0        0        0     3099 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/README.md
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/bower.json
+-rwxr-xr-x   0        0        0    27045 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/excanvas.js
+-rwxr-xr-x   0        0        0    13014 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/index.html
+-rwxr-xr-x   0        0        0      984 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/knob.jquery.json
+-rwxr-xr-x   0        0        0      589 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/package.json
+-rwxr-xr-x   0        0        0    33487 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/secretplan.jpg
+-rwxr-xr-x   0        0        0    26225 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/js/jquery.knob.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/js-synthesizer/.gitignore
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/js-synthesizer/README.txt
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/js-synthesizer/demo.html
+-rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/js-synthesizer/instruments.js
+-rw-r--r--   0        0        0    11184 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/js-synthesizer/synthesis.js
+-rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/platform-1.3.6/platform.min.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/raphael-2.3.0/.eslintrc.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/raphael-2.3.0/.gitignore
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/raphael-2.3.0/README.md
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/raphael-2.3.0/license.txt
+-rw-r--r--   0        0        0    93167 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/libraries/raphael-2.3.0/raphael.min.js
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/scripts/dashboard_timeline.js
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/resources/scripts/prepare_docker_image.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/abort_not_possible.html
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/abort_possible.html
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/ad.html
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consent.html
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/dashboard_timeline.html
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/exit_recruiter_lucid.html
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/final-page-bonuses.html
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/final-page-rejected-consent.html
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/final-page-successful.html
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/final-page-unsuccessful.html
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/info-page.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/macros.html
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/mturk_error.html
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/participant.html
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/psynet_layout.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/questions.html
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/resume.html
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/start.html
+-rw-r--r--   0        0        0    67246 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/timeline-page.html
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/unity-debug-page.html
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/unity-page.html
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/wait-page.html
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/audiovisual_consent.html
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/cap-recruiter_audiovisual_consent.html
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/cap-recruiter_standard_consent.html
+-rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/database_consent.html
+-rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/main_consent.html
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/mturk_audiovisual_consent.html
+-rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/mturk_standard_consent.html
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/open_science_consent.html
+-rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/princeton_cap_recruiter_consent.html
+-rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/princeton_consent.html
+-rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/consents/voluntary_with_no_compensation_consent.html
+-rw-r--r--   0        0        0    62854 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/macros/control.html
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/macros/graphics.html
+-rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/macros/prompt.html
+-rw-r--r--   0        0        0   194322 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/macros/control/RecordRTC.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/macros/control/__init__.py
+-rw-r--r--   0        0        0   199443 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/macros/control/adapter.js
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/macros/control/audio_meter.js
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/templates/macros/control/recorder.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/__init__.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/audio.py
+-rw-r--r--   0        0        0    15679 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/audio_gibbs.py
+-rw-r--r--   0        0        0    52506 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/chain.py
+-rw-r--r--   0        0        0    30793 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/dense.py
+-rw-r--r--   0        0        0    12498 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/gibbs.py
+-rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/graph.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/imitation_chain.py
+-rw-r--r--   0        0        0    88618 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/main.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/mcmcp.py
+-rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/record.py
+-rw-r--r--   0        0        0    57654 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/static.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 psynet-9.4.6/psynet/trial/video.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 psynet-9.4.6/.gitignore
+-rwxr-xr-x   0        0        0     1126 2020-02-02 00:00:00.000000 psynet-9.4.6/LICENSE
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 psynet-9.4.6/README.md
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 psynet-9.4.6/pyproject.toml
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 psynet-9.4.6/PKG-INFO
```

### Comparing `psynet-9.4.5/.gitlab-ci.yml` & `psynet-9.4.6/.gitlab-ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 image: python:3.10
 
-# Originally we used the GitLab Postgres service.
-# However, it seemed to be a bit buggy, so we are now installing
-# Postgres locally. Here is the config that we used to use:
-#
-#services:
-#  - postgres:12.2-alpine
-#
-#variables:
-#  POSTGRES_DB: dallinger
-#  POSTGRES_USER: dallinger
-#  POSTGRES_PASSWORD: ""
-#  POSTGRES_HOST_AUTH_METHOD: trust
-#  DATABASE_URL: postgresql://dallinger@postgres:5432/dallinger
+# Comment this out if you decide to use local postgres instead
+services:
+  - postgres:12.2-alpine
 
+# Comment this out if you decide to use local postgres instead
 variables:
   POSTGRES_DB: dallinger
   POSTGRES_USER: dallinger
-  POSTGRES_PASSWORD: "dallinger"
-  DATABASE_URL: postgresql://dallinger:dallinger@localhost:5432/dallinger
+  POSTGRES_PASSWORD: ""
+  POSTGRES_HOST_AUTH_METHOD: trust
+  DATABASE_URL: postgresql://dallinger@postgres:5432/dallinger
+
+# Uncomment this if you decide to use local postgres instead
+#variables:
+#  POSTGRES_DB: dallinger
+#  POSTGRES_USER: dallinger
+#  POSTGRES_PASSWORD: "dallinger"
+#  DATABASE_URL: postgresql://dallinger:dallinger@localhost:5432/dallinger
 
 before_script:
 # General setup
   - apt update
   - apt -f -y install curl redis-server unzip
   - service redis-server start
   - curl https://cli-assets.heroku.com/install.sh | sh
   - wget -O chrome.deb http://dl.google.com/linux/chrome/deb/pool/main/g/google-chrome-stable/google-chrome-stable_109.0.5414.74-1_amd64.deb
   - wget -O chrome-driver.zip https://chromedriver.storage.googleapis.com/109.0.5414.74/chromedriver_linux64.zip
   - apt -f -y install ./chrome.deb
   - unzip chrome-driver.zip chromedriver -d /usr/local/bin/
   - pip install "git+https://gitlab+deploy-token-478431:98jnkW1yq_AYWLYpRNtN@gitlab.com/computational-audition-lab/melody/melody-experiments@master#egg=melody_experiments[extract]"
   - pip install pytest-test-groups
   - export HEADLESS=TRUE
-# Install and setup PostgreSQL
-  - apt install -y postgresql postgresql-contrib libpq-dev
-  - service postgresql start
-  - runuser -l postgres -c 'echo -e "dallinger\ndallinger" | createuser -P -e dallinger'
-  - chown postgres:postgres postgres_setup.sql
-  - runuser -l postgres -c 'psql -c "\i /builds/PsyNetDev/PsyNet/postgres_setup.sql"'
+# Install and setup PostgreSQL - uncomment this if you decide to use local postgres instead
+#  - apt install -y postgresql postgresql-contrib libpq-dev
+#  - service postgresql start
+#  - runuser -l postgres -c 'echo -e "dallinger\ndallinger" | createuser -P -e dallinger'
+#  - chown postgres:postgres postgres_setup.sql
+#  - runuser -l postgres -c 'psql -c "\i /builds/PsyNetDev/PsyNet/postgres_setup.sql"'
 # Install Dallinger
-  - git clone --branch v9.6.0 https://github.com/Dallinger/Dallinger.git /tmp/dallinger
+  - git clone --branch v9.8.2 https://github.com/Dallinger/Dallinger.git /tmp/dallinger
   - pip install -r /tmp/dallinger/dev-requirements.txt
   - pip install -e '/tmp/dallinger[data]'
 # Install PsyNet
   - pip install -e '.[dev]'
 
 tests:
   parallel: 5
```

### Comparing `psynet-9.4.5/CHANGELOG.md` & `psynet-9.4.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # CHANGELOG
 
+# [9.4.6] Released on 2023-07-06
+
+#### Fixed
+- Use `jquery.knob.js` instead of `jquery.knob.min.js` to avoid manifest problems (author: Peter Harrison).
+- Fixed CI problems by reverting to Postgres as a service (author: Peter Harrison).
+
+#### Updated
+- Updated `Dallinger` to `v9.8.2`. See the complete release notes at https://github.com/Dallinger/Dallinger/releases/tag/v9.8.2.
+
 # [9.4.5] Released on 2023-04-24
 
 #### Fixed
 - Added a random key to Unity assets to avoid caching in the browser (author: Pol van Rijn, reviewer: Frank Höger).
 
 #### Added
 - Added `BigFiveQuestionnaire` and `AltruismQuestionnaire` (author: Pol van Rijn, reviewer: Frank Höger).
```

### Comparing `psynet-9.4.5/MANIFEST.in` & `psynet-9.4.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/unity_interface_description.md` & `psynet-9.4.6/unity_interface_description.md`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/audio_mixer.py` & `psynet-9.4.6/psynet/audio_mixer.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/bot.py` & `psynet-9.4.6/psynet/bot.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/command_line.py` & `psynet-9.4.6/psynet/command_line.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/consent.py` & `psynet-9.4.6/psynet/consent.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/data.py` & `psynet-9.4.6/psynet/data.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/experiment.py` & `psynet-9.4.6/psynet/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -776,17 +776,17 @@
                 resource_filename(
                     "psynet", "resources/libraries/raphael-2.3.0/raphael.min.js"
                 ),
                 "/static/scripts/raphael-2.3.0.min.js",
             ),
             (
                 resource_filename(
-                    "psynet", "resources/libraries/jQuery-Knob/dist/jquery.knob.min.js"
+                    "psynet", "resources/libraries/jQuery-Knob/js/jquery.knob.js"
                 ),
-                "/static/scripts/jquery.knob.min.js",
+                "/static/scripts/jquery.knob.js",
             ),
             (
                 resource_filename("psynet", "resources/libraries/js-synthesizer"),
                 "/static/scripts/js-synthesizer",
             ),
             (
                 resource_filename("psynet", "resources/libraries/Tonejs"),
```

### Comparing `psynet-9.4.5/psynet/field.py` & `psynet-9.4.6/psynet/field.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/graphics.py` & `psynet-9.4.6/psynet/graphics.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/js_synth.py` & `psynet-9.4.6/psynet/js_synth.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/lucid.py` & `psynet-9.4.6/psynet/lucid.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/media.py` & `psynet-9.4.6/psynet/media.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/modular_page.py` & `psynet-9.4.6/psynet/modular_page.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/page.py` & `psynet-9.4.6/psynet/page.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/participant.py` & `psynet-9.4.6/psynet/participant.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/prescreen.py` & `psynet-9.4.6/psynet/prescreen.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/recruiters.py` & `psynet-9.4.6/psynet/recruiters.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/test.py` & `psynet-9.4.6/psynet/test.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/timeline.py` & `psynet-9.4.6/psynet/timeline.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/utils.py` & `psynet-9.4.6/psynet/utils.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/definitions/gold-msi.csv` & `psynet-9.4.6/psynet/definitions/gold-msi.csv`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/demography/general.py` & `psynet-9.4.6/psynet/demography/general.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/demography/gmsi.py` & `psynet-9.4.6/psynet/demography/gmsi.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/demography/pei.py` & `psynet-9.4.6/psynet/demography/pei.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/favicon.ico` & `psynet-9.4.6/psynet/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/logo.png` & `psynet-9.4.6/psynet/resources/logo.png`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/logo.svg` & `psynet-9.4.6/psynet/resources/logo.svg`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/logo_image_only.png` & `psynet-9.4.6/psynet/resources/logo_image_only.png`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/css/dashboard_timeline.css` & `psynet-9.4.6/psynet/resources/css/dashboard_timeline.css`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/images/princeton-consent.png` & `psynet-9.4.6/psynet/resources/images/princeton-consent.png`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/images/unity_logo.png` & `psynet-9.4.6/psynet/resources/images/unity_logo.png`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/Tonejs/LICENSE.md` & `psynet-9.4.6/psynet/resources/libraries/Tonejs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/Tonejs/Tone.js` & `psynet-9.4.6/psynet/resources/libraries/Tonejs/Tone.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/jQuery/jquery-3.6.0.min.js` & `psynet-9.4.6/psynet/resources/libraries/jQuery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/LICENSE` & `psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/LICENSE`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/README.md` & `psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/README.md`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/excanvas.js` & `psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/excanvas.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/index.html` & `psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/index.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/knob.jquery.json` & `psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/knob.jquery.json`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/package.json` & `psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/package.json`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/secretplan.jpg` & `psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/secretplan.jpg`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/js/jquery.knob.js` & `psynet-9.4.6/psynet/resources/libraries/jQuery-Knob/js/jquery.knob.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/js-synthesizer/README.txt` & `psynet-9.4.6/psynet/resources/libraries/js-synthesizer/README.txt`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/js-synthesizer/demo.html` & `psynet-9.4.6/psynet/resources/libraries/js-synthesizer/demo.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/js-synthesizer/instruments.js` & `psynet-9.4.6/psynet/resources/libraries/js-synthesizer/instruments.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/js-synthesizer/synthesis.js` & `psynet-9.4.6/psynet/resources/libraries/js-synthesizer/synthesis.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/platform-1.3.6/platform.min.js` & `psynet-9.4.6/psynet/resources/libraries/platform-1.3.6/platform.min.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/README.md` & `psynet-9.4.6/psynet/resources/libraries/raphael-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/license.txt` & `psynet-9.4.6/psynet/resources/libraries/raphael-2.3.0/license.txt`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/raphael.min.js` & `psynet-9.4.6/psynet/resources/libraries/raphael-2.3.0/raphael.min.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/scripts/dashboard_timeline.js` & `psynet-9.4.6/psynet/resources/scripts/dashboard_timeline.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/resources/scripts/prepare_docker_image.sh` & `psynet-9.4.6/psynet/resources/scripts/prepare_docker_image.sh`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/abort_not_possible.html` & `psynet-9.4.6/psynet/templates/abort_not_possible.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/abort_possible.html` & `psynet-9.4.6/psynet/templates/abort_possible.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/ad.html` & `psynet-9.4.6/psynet/templates/ad.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consent.html` & `psynet-9.4.6/psynet/templates/consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/dashboard_timeline.html` & `psynet-9.4.6/psynet/templates/dashboard_timeline.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/exit_recruiter_lucid.html` & `psynet-9.4.6/psynet/templates/exit_recruiter_lucid.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/final-page-unsuccessful.html` & `psynet-9.4.6/psynet/templates/final-page-unsuccessful.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/mturk_error.html` & `psynet-9.4.6/psynet/templates/mturk_error.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/participant.html` & `psynet-9.4.6/psynet/templates/participant.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/psynet_layout.html` & `psynet-9.4.6/psynet/templates/psynet_layout.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/resume.html` & `psynet-9.4.6/psynet/templates/resume.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/start.html` & `psynet-9.4.6/psynet/templates/start.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/timeline-page.html` & `psynet-9.4.6/psynet/templates/timeline-page.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/unity-debug-page.html` & `psynet-9.4.6/psynet/templates/unity-debug-page.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/unity-page.html` & `psynet-9.4.6/psynet/templates/unity-page.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/wait-page.html` & `psynet-9.4.6/psynet/templates/wait-page.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/audiovisual_consent.html` & `psynet-9.4.6/psynet/templates/consents/audiovisual_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/cap-recruiter_audiovisual_consent.html` & `psynet-9.4.6/psynet/templates/consents/cap-recruiter_audiovisual_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/cap-recruiter_standard_consent.html` & `psynet-9.4.6/psynet/templates/consents/cap-recruiter_standard_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/database_consent.html` & `psynet-9.4.6/psynet/templates/consents/database_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/main_consent.html` & `psynet-9.4.6/psynet/templates/consents/main_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/mturk_audiovisual_consent.html` & `psynet-9.4.6/psynet/templates/consents/mturk_audiovisual_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/mturk_standard_consent.html` & `psynet-9.4.6/psynet/templates/consents/mturk_standard_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/open_science_consent.html` & `psynet-9.4.6/psynet/templates/consents/open_science_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/princeton_cap_recruiter_consent.html` & `psynet-9.4.6/psynet/templates/consents/princeton_cap_recruiter_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/princeton_consent.html` & `psynet-9.4.6/psynet/templates/consents/princeton_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/consents/voluntary_with_no_compensation_consent.html` & `psynet-9.4.6/psynet/templates/consents/voluntary_with_no_compensation_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/macros/control.html` & `psynet-9.4.6/psynet/templates/macros/control.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/macros/graphics.html` & `psynet-9.4.6/psynet/templates/macros/graphics.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/macros/prompt.html` & `psynet-9.4.6/psynet/templates/macros/prompt.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/macros/control/RecordRTC.js` & `psynet-9.4.6/psynet/templates/macros/control/RecordRTC.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/macros/control/adapter.js` & `psynet-9.4.6/psynet/templates/macros/control/adapter.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/macros/control/audio_meter.js` & `psynet-9.4.6/psynet/templates/macros/control/audio_meter.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/templates/macros/control/recorder.js` & `psynet-9.4.6/psynet/templates/macros/control/recorder.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/audio.py` & `psynet-9.4.6/psynet/trial/audio.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/audio_gibbs.py` & `psynet-9.4.6/psynet/trial/audio_gibbs.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/chain.py` & `psynet-9.4.6/psynet/trial/chain.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/dense.py` & `psynet-9.4.6/psynet/trial/dense.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/gibbs.py` & `psynet-9.4.6/psynet/trial/gibbs.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/graph.py` & `psynet-9.4.6/psynet/trial/graph.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/imitation_chain.py` & `psynet-9.4.6/psynet/trial/imitation_chain.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/main.py` & `psynet-9.4.6/psynet/trial/main.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/mcmcp.py` & `psynet-9.4.6/psynet/trial/mcmcp.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/record.py` & `psynet-9.4.6/psynet/trial/record.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/static.py` & `psynet-9.4.6/psynet/trial/static.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/psynet/trial/video.py` & `psynet-9.4.6/psynet/trial/video.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/.gitignore` & `psynet-9.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/LICENSE` & `psynet-9.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/README.md` & `psynet-9.4.6/README.md`

 * *Files identical despite different names*

### Comparing `psynet-9.4.5/pyproject.toml` & `psynet-9.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "psynet"
-version = "9.4.5"
+version = "9.4.6"
 authors = [
   { name="Peter Harrison", email="pmch2@cam.ac.uk" },
   { name="Frank Höger", email="frank.hoeger@ae.mpg.de" },
   { name="Pol van Rijn", email="pol.van-rijn@ae.mpg.de" },
   { name="Raja Marjieh", email="raja.marjieh@princeton.edu" },
   { name="Nori Jacoby", email="nori.jacoby@ae.mpg.de" }
 ]
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3",
     "Framework :: Flask",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Science/Research",
 ]
 dependencies = [
-    "dallinger>=9.6.0, <10",
+    "dallinger>=9.8.2, <10",
     "dominate",
     "importlib_resources",
     "joblib",
     "jsonpickle",
     "paramiko",
     "praat-parselmouth",
     "progress",
```

### Comparing `psynet-9.4.5/PKG-INFO` & `psynet-9.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psynet
-Version: 9.4.5
+Version: 9.4.6
 Summary: PsyNet – The online human behaviour lab of the future
 Project-URL: Changelog, https://gitlab.com/PsyNetDev/PsyNet/-/blob/v9-master/CHANGELOG.md
 Project-URL: Documentation, https://psynetdev.gitlab.io/PsyNet/
 Project-URL: Homepage, https://www.psynet.dev/
 Project-URL: Issues, https://gitlab.com/PsyNetDev/PsyNet/-/issues
 Project-URL: Repository, https://gitlab.com/PsyNetDev/PsyNet/-/tree/v9-master
 Author-email: Peter Harrison <pmch2@cam.ac.uk>, Frank Höger <frank.hoeger@ae.mpg.de>, Pol van Rijn <pol.van-rijn@ae.mpg.de>, Raja Marjieh <raja.marjieh@princeton.edu>, Nori Jacoby <nori.jacoby@ae.mpg.de>
@@ -29,15 +29,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: dallinger<10,>=9.6.0
+Requires-Dist: dallinger<10,>=9.8.2
 Requires-Dist: dominate
 Requires-Dist: importlib-resources
 Requires-Dist: joblib
 Requires-Dist: jsonpickle
 Requires-Dist: paramiko
 Requires-Dist: praat-parselmouth
 Requires-Dist: progress
```

