# Comparing `tmp/schwifty-2024.5.3.tar.gz` & `tmp/schwifty-2024.5.4.tar.gz`

## Comparing `schwifty-2024.5.3.tar` & `schwifty-2024.5.4.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 schwifty-2024.5.3/.envrc
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schwifty-2024.5.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 schwifty-2024.5.3/.readthedocs.yml
--rw-r--r--   0        0        0    21732 2020-02-02 00:00:00.000000 schwifty-2024.5.3/CHANGELOG.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 schwifty-2024.5.3/Makefile
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 schwifty-2024.5.3/devbox.json
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.3/devbox.lock
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 schwifty-2024.5.3/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 schwifty-2024.5.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 schwifty-2024.5.3/docs/Makefile
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 schwifty-2024.5.3/docs/requirements.txt
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 schwifty-2024.5.3/docs/source/api.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 schwifty-2024.5.3/docs/source/changelog.rst
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 schwifty-2024.5.3/docs/source/conf.py
--rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 schwifty-2024.5.3/docs/source/examples.rst
--rw-r--r--   0        0        0   366898 2020-02-02 00:00:00.000000 schwifty-2024.5.3/docs/source/ilikewhatugot.png
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 schwifty-2024.5.3/docs/source/index.rst
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 schwifty-2024.5.3/docs/source/troubleshooting.rst
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/__init__.py
--rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bban.py
--rw-r--r--   0        0        0    16894 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bic.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/common.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/domain.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/exceptions.py
--rw-r--r--   0        0        0    16158 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/iban.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/py.typed
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/registry.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/README.md
--rw-r--r--   0        0        0   191535 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_at.json
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_ba.json
--rw-r--r--   0        0        0   134356 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_be.json
--rw-r--r--   0        0        0   218276 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_ch.json
--rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_cz.json
--rw-r--r--   0        0        0  1064251 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_de.json
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_ee.json
--rw-r--r--   0        0        0   105235 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_es.json
--rw-r--r--   0        0        0   123774 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_fi.json
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_ge.json
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_hr.json
--rw-r--r--   0        0        0    31389 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_hu.json
--rw-r--r--   0        0        0    59696 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_it.json
--rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_kz.json
--rw-r--r--   0        0        0    56450 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_lt.json
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_lv.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_md.json
--rw-r--r--   0        0        0    14272 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_nl.json
--rw-r--r--   0        0        0   406123 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_no.json
--rw-r--r--   0        0        0   768164 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_pl.json
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_ro.json
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_rs.json
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_se.json
--rw-r--r--   0        0        0   145633 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_si.json
--rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_sk.json
--rw-r--r--   0        0        0  1752206 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/generated_ua.json
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_ad.json
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_ae.json
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_bg.json
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_cr.json
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_cy.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_dk.json
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_es.json
--rw-r--r--   0        0        0    68361 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_fr.json
--rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_gb.json
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_gr.json
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_ie.json
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_il.json
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_is.json
--rw-r--r--   0        0        0    26893 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_it.json
--rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_lu.json
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_mc.json
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_me.json
--rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_pt.json
--rw-r--r--   0        0        0    25035 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_sa.json
--rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/bank_registry/manual_tr.json
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/__init__.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/albania.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/belgium.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/czech_republic.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/estonia.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/finland.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/france.py
--rw-r--r--   0        0        0    15549 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/germany.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/iceland.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/iso7064_mod97_10.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/iso7064_mod97_10_variant.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/italy.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/netherlands.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/norway.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/poland.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/registry.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/checksum/spain.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/iban_registry/README.md
--rw-r--r--   0        0        0    33306 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/iban_registry/generated.json
--rw-r--r--   0        0        0    16740 2020-02-02 00:00:00.000000 schwifty-2024.5.3/schwifty/iban_registry/overwrite.json
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/Dockerfile_se
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/README.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_at.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_be.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_ch.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_cz.py
--rwxr-xr-x   0        0        0     2066 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_de.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_es.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_fi.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_hr.py
--rwxr-xr-x   0        0        0     1213 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_hu.py
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_it.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_lt.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_lv.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_nl.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_no.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_pl.py
--rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_ro.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_se.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_si.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_sk.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_bank_registry_ua.py
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/get_iban_registry.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/requirements.txt
--rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 schwifty-2024.5.3/scripts/update-all.sh
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 schwifty-2024.5.3/tests/test_bban.py
--rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 schwifty-2024.5.3/tests/test_bic.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 schwifty-2024.5.3/tests/test_checksum.py
--rw-r--r--   0        0        0    15576 2020-02-02 00:00:00.000000 schwifty-2024.5.3/tests/test_iban.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 schwifty-2024.5.3/tests/test_registry.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 schwifty-2024.5.3/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 schwifty-2024.5.3/LICENSE
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 schwifty-2024.5.3/README.rst
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 schwifty-2024.5.3/hatch.toml
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 schwifty-2024.5.3/pyproject.toml
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 schwifty-2024.5.3/PKG-INFO
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 schwifty-2024.5.4/.envrc
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schwifty-2024.5.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 schwifty-2024.5.4/.readthedocs.yml
+-rw-r--r--   0        0        0    22507 2020-02-02 00:00:00.000000 schwifty-2024.5.4/CHANGELOG.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 schwifty-2024.5.4/Makefile
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 schwifty-2024.5.4/devbox.json
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 schwifty-2024.5.4/devbox.lock
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 schwifty-2024.5.4/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 schwifty-2024.5.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 schwifty-2024.5.4/docs/Makefile
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 schwifty-2024.5.4/docs/requirements.txt
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 schwifty-2024.5.4/docs/source/api.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 schwifty-2024.5.4/docs/source/changelog.rst
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 schwifty-2024.5.4/docs/source/conf.py
+-rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 schwifty-2024.5.4/docs/source/examples.rst
+-rw-r--r--   0        0        0   366898 2020-02-02 00:00:00.000000 schwifty-2024.5.4/docs/source/ilikewhatugot.png
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 schwifty-2024.5.4/docs/source/index.rst
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 schwifty-2024.5.4/docs/source/troubleshooting.rst
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/__init__.py
+-rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bban.py
+-rw-r--r--   0        0        0    17038 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bic.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/common.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/domain.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/exceptions.py
+-rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/iban.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/py.typed
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/registry.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/README.md
+-rw-r--r--   0        0        0   191535 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_at.json
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_ba.json
+-rw-r--r--   0        0        0   134356 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_be.json
+-rw-r--r--   0        0        0   218276 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_ch.json
+-rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_cz.json
+-rw-r--r--   0        0        0  1064251 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_de.json
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_ee.json
+-rw-r--r--   0        0        0   105235 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_es.json
+-rw-r--r--   0        0        0   123774 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_fi.json
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_ge.json
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_hr.json
+-rw-r--r--   0        0        0    31389 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_hu.json
+-rw-r--r--   0        0        0    59696 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_it.json
+-rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_kz.json
+-rw-r--r--   0        0        0    56450 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_lt.json
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_lv.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_md.json
+-rw-r--r--   0        0        0    14272 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_nl.json
+-rw-r--r--   0        0        0   406123 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_no.json
+-rw-r--r--   0        0        0   768164 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_pl.json
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_ro.json
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_rs.json
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_se.json
+-rw-r--r--   0        0        0   145633 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_si.json
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_sk.json
+-rw-r--r--   0        0        0  1752206 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/generated_ua.json
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_ad.json
+-rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_ae.json
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_bg.json
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_cr.json
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_cy.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_dk.json
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_es.json
+-rw-r--r--   0        0        0    68361 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_fr.json
+-rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_gb.json
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_gr.json
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_ie.json
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_il.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_is.json
+-rw-r--r--   0        0        0    26893 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_it.json
+-rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_lu.json
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_mc.json
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_me.json
+-rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_pt.json
+-rw-r--r--   0        0        0    25035 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_sa.json
+-rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/bank_registry/manual_tr.json
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/__init__.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/albania.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/belgium.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/czech_republic.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/estonia.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/finland.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/france.py
+-rw-r--r--   0        0        0    15549 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/germany.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/iceland.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/iso7064_mod97_10.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/iso7064_mod97_10_variant.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/italy.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/netherlands.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/norway.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/poland.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/registry.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/checksum/spain.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/iban_registry/README.md
+-rw-r--r--   0        0        0    33306 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/iban_registry/generated.json
+-rw-r--r--   0        0        0    17073 2020-02-02 00:00:00.000000 schwifty-2024.5.4/schwifty/iban_registry/overwrite.json
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/Dockerfile_se
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/README.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_at.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_be.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_ch.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_cz.py
+-rwxr-xr-x   0        0        0     2066 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_de.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_es.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_fi.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_hr.py
+-rwxr-xr-x   0        0        0     1213 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_hu.py
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_it.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_lt.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_lv.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_nl.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_no.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_pl.py
+-rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_ro.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_se.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_si.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_sk.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_bank_registry_ua.py
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/get_iban_registry.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/requirements.txt
+-rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 schwifty-2024.5.4/scripts/update-all.sh
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 schwifty-2024.5.4/tests/test_bban.py
+-rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 schwifty-2024.5.4/tests/test_bic.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 schwifty-2024.5.4/tests/test_checksum.py
+-rw-r--r--   0        0        0    16278 2020-02-02 00:00:00.000000 schwifty-2024.5.4/tests/test_iban.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 schwifty-2024.5.4/tests/test_registry.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 schwifty-2024.5.4/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 schwifty-2024.5.4/LICENSE
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 schwifty-2024.5.4/README.rst
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 schwifty-2024.5.4/hatch.toml
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 schwifty-2024.5.4/pyproject.toml
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 schwifty-2024.5.4/PKG-INFO
```

### Comparing `schwifty-2024.5.3/CHANGELOG.rst` & `schwifty-2024.5.4/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 .. _changelog:
 
 Changelog
 =========
 
 Versions follow `CalVer <http://www.calver.org/>`_ with the scheme ``YY.0M.Micro``.
 
+`2024.05.4`_ - 2024/05/25
+-------------------------
+Added
+~~~~~
+* The ``IBAN`` and ``BBAN`` classes now have an additional property ``currency_code`` for countries
+  like Seychelles, Guatemala or Mauritius.
+
+Fixed
+~~~~~
+* Also allow the BIC lookup for non-primary banks. For countries like Switzerland the lookup did
+  fail for banks which did not have the primary-flag set, even though an appropriate mapping was
+  available.
+* ``IBAN.random()`` now also works for countries which have a currency code included in their BBAN
+  e.g. Mauritius or Seychelles.
+* ``IBAN.random()`` now also works for aspirational countries, where no information of the BBAN
+  structure is available, e.g. Comoros.
+
 `2024.05.3`_ - 2024/05/10
 -------------------------
 Added
 ~~~~~
 * There is a new classmethod ``IBAN.random()`` that allows you to create random, but valid IBANs.
 
   .. code-block:: pycon
@@ -619,14 +636,15 @@
 -------------------------
 
 Added
 ~~~~~
 * Added :attr:`.BIC.country` and :attr:`.IBAN.country`.
 
 
+.. _2024.05.4: https://github.com/mdomke/schwifty/compare/2024.05.3...2024.05.4
 .. _2024.05.3: https://github.com/mdomke/schwifty/compare/2024.05.2...2024.05.3
 .. _2024.05.2: https://github.com/mdomke/schwifty/compare/2024.05.1...2024.05.2
 .. _2024.05.1: https://github.com/mdomke/schwifty/compare/2024.05.0...2024.05.1
 .. _2024.05.0: https://github.com/mdomke/schwifty/compare/2024.04.0...2024.05.0
 .. _2024.04.0: https://github.com/mdomke/schwifty/compare/2024.01.1...2024.04.0
 .. _2024.01.1: https://github.com/mdomke/schwifty/compare/2023.11.2...2024.01.1
 .. _2023.11.2: https://github.com/mdomke/schwifty/compare/2023.11.1...2023.11.2
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_tjbyyh0i_/tmp1qmr_wz5_TarContainer/0/3.rst", line 674, column 0: CDATA terminal not found*

```diff
@@ -1,12 +1,21 @@
 .. _changelog: Changelog ========= Versions follow `CalVer
-www.calver.org/>`_ with the scheme ``YY.0M.Micro``. `2024.05.3`_ - 2024/05/10 -
------------------------- Added ~~~~~ * There is a new classmethod ``IBAN.random
-()`` that allows you to create random, but valid IBANs. .. code-block:: pycon
->>> IBAN.random()
+www.calver.org/>`_ with the scheme ``YY.0M.Micro``. `2024.05.4`_ - 2024/05/25 -
+------------------------ Added ~~~~~ * The ``IBAN`` and ``BBAN`` classes now
+have an additional property ``currency_code`` for countries like Seychelles,
+Guatemala or Mauritius. Fixed ~~~~~ * Also allow the BIC lookup for non-primary
+banks. For countries like Switzerland the lookup did fail for banks which did
+not have the primary-flag set, even though an appropriate mapping was
+available. * ``IBAN.random()`` now also works for countries which have a
+currency code included in their BBAN e.g. Mauritius or Seychelles. *
+``IBAN.random()`` now also works for aspirational countries, where no
+information of the BBAN structure is available, e.g. Comoros. `2024.05.3`_ -
+2024/05/10 ------------------------- Added ~~~~~ * There is a new classmethod
+``IBAN.random()`` that allows you to create random, but valid IBANs. .. code-
+block:: pycon >>> IBAN.random()
 LT435012771675726758> You can narrow down the generated values by providing the
 corresponding parameters to this function. E.g. to get only Spanish IBANs you
 can do .. code-block:: pycon >>> IBAN.random(country_code="ES")
 ES8801253179194914182449> Changed ~~~~~~~ * Some missing bank associations have
 been added to the Portoguese bank registry by `@tiagoafseixas
 github.com/tiagoafseixas>`_ `2024.05.2`_ - 2024/05/09 ------------------------
 - Fixed ~~~~~ * Add `typing-extensions` as explicit dependency for Python <
```

### Comparing `schwifty-2024.5.3/.github/workflows/lint-and-test.yml` & `schwifty-2024.5.4/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/.github/workflows/publish.yml` & `schwifty-2024.5.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/docs/Makefile` & `schwifty-2024.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/docs/source/api.rst` & `schwifty-2024.5.4/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/docs/source/conf.py` & `schwifty-2024.5.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/docs/source/examples.rst` & `schwifty-2024.5.4/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/docs/source/ilikewhatugot.png` & `schwifty-2024.5.4/docs/source/ilikewhatugot.png`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/docs/source/index.rst` & `schwifty-2024.5.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/docs/source/troubleshooting.rst` & `schwifty-2024.5.4/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bban.py` & `schwifty-2024.5.4/schwifty/bban.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,23 +189,28 @@
 
         rstr = Rstr(random)
         spec = _get_bban_spec(country_code)
         bank: dict[str, Any] = {}
         if (banks := banks_by_country.get(country_code)) is not None and use_registry:
             bank = random.choice(banks)
 
+        if "positions" not in spec:
+            return cls(country_code, rstr.xeger(spec["regex"]).upper())
+
         ranges = _get_position_ranges(spec)
         for _ in range(100):
             bban = rstr.xeger(spec["regex"]).upper()
             components: dict[Component, str] = {}
             for key, range_ in ranges.items():
                 if (value := values.get(key)) is not None:
                     components[key] = value
                 else:
-                    components[key] = bank.get(key) or range_.cut(bban)
+                    components[key] = bank.get(key) or spec.get(
+                        f"default_{key.value}", range_.cut(bban)
+                    )
 
             bank_code = components[Component.BANK_CODE]
             bank_code_length = ranges[Component.BANK_CODE].length
             branch_code_length = ranges[Component.BRANCH_CODE].length
 
             if len(bank_code) >= bank_code_length + branch_code_length:
                 start = bank_code_length
@@ -303,14 +308,22 @@
         """str: Account holder's national identification.
 
         This value is only available for Iceland.
         """
         return self._get_component(Component.ACCOUNT_HOLDER_ID)
 
     @property
+    def currency_code(self) -> str:
+        """str: The account's currency code.
+
+        This value is only available for Mauretania, Seychelles and Guatemala.
+        """
+        return self._get_component(Component.CURRENCY_CODE)
+
+    @property
     def bank(self) -> dict | None:
         """dict | None: The information of bank related to this BBANs bank code."""
         bank_registry = registry.get("bank_code")
         assert isinstance(bank_registry, dict)
 
         lookup_by = self.spec.get("bic_lookup_components", [Component.BANK_CODE])
         key = "".join(self._get_component(component) for component in lookup_by)
```

### Comparing `schwifty-2024.5.3/schwifty/bic.py` & `schwifty-2024.5.4/schwifty/bic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import re
 import warnings
+from operator import itemgetter
 from typing import Any
 from typing import TYPE_CHECKING
 
 from pycountry import countries  # type: ignore
 from pycountry.db import Data  # type: ignore
 
 from schwifty import common
@@ -163,17 +164,20 @@
             * Switzerland
             * Turkiye
             * Ukraine
             * United Arab Emirates
             * United Kingdom
         """
         try:
-            spec = registry.get("bank_code")
-            assert isinstance(spec, dict)
-            return [cls(entry["bic"]) for entry in spec[(country_code, bank_code)]]
+            index = registry.get("bank_code")
+            assert isinstance(index, dict)
+            banks = sorted(
+                index[(country_code, bank_code)], key=itemgetter("primary"), reverse=True
+            )
+            return [cls(entry["bic"]) for entry in banks]
         except KeyError as e:
             raise exceptions.InvalidBankCode(
                 f"Unknown bank code {bank_code!r} for country {country_code!r}"
             ) from e
 
     @classmethod
     def from_bank_code(cls, country_code: str, bank_code: str) -> BIC:
@@ -489,15 +493,14 @@
 
     @property
     def branch_code(self) -> str:
         """str: The branch-code part of the BIC (if available)"""
         return self._get_slice(start=8, end=11)
 
 
-registry.build_index("bank", "bic", key="bic", accumulate=True)
+registry.build_index("bank", index_name="bic", key="bic", accumulate=True)
 registry.build_index(
     "bank",
-    "bank_code",
+    index_name="bank_code",
     key=("country_code", "bank_code"),
-    primary=True,
     accumulate=True,
 )
```

### Comparing `schwifty-2024.5.3/schwifty/common.py` & `schwifty-2024.5.4/schwifty/common.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/exceptions.py` & `schwifty-2024.5.4/schwifty/exceptions.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/iban.py` & `schwifty-2024.5.4/schwifty/iban.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,14 +369,22 @@
         """str: Account holder's national identification.
 
         This value is only available for Iceland.
         """
         return self.bban.account_holder_id
 
     @property
+    def currency_code(self) -> str:
+        """str: The account's currency code.
+
+        This value is only available for Mauretania, Seychelles and Guatemala.
+        """
+        return self.bban.currency_code
+
+    @property
     def bank(self) -> dict | None:
         """dict or None: The information of the bank related to the bank code as part of the BBAN"""
         return self.bban.bank
 
     @property
     def bank_name(self) -> str | None:
         """str or None: The name of the bank associated with the IBAN bank code.
@@ -438,19 +446,23 @@
             iban = cls(value)
         except exceptions.SchwiftyException as err:
             raise PydanticCustomError("iban_format", str(err)) from err
         return handler(iban)
 
 
 def add_bban_regex(country: str, spec: dict) -> dict:
-    bban_spec = spec["bban_spec"]
+    if "regex" not in spec:
+        spec["regex"] = re.compile(convert_bban_spec_to_regex(spec["bban_spec"]))
+    return spec
+
+
+def convert_bban_spec_to_regex(spec: str) -> str:
     spec_re = rf"(\d+)(!)?([{''.join(_spec_to_re.keys())}])"
 
     def convert(match: re.Match) -> str:
         quantifier = ("{{{}}}" if match.group(2) else "{{1,{}}}").format(match.group(1))
         return _spec_to_re[match.group(3)] + quantifier
 
-    spec["regex"] = re.compile(rf"^{re.sub(spec_re, convert, bban_spec)}$")
-    return spec
+    return rf"^{re.sub(spec_re, convert, spec)}$"
 
 
 registry.manipulate("iban", add_bban_regex)
```

### Comparing `schwifty-2024.5.3/schwifty/registry.py` & `schwifty-2024.5.4/schwifty/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,24 +75,26 @@
     accumulate: bool = False,
     **predicate: Any,
 ) -> None:
     def make_key(entry: dict[Key, Any]) -> tuple | str:
         return tuple(entry[k] for k in key) if isinstance(key, tuple) else entry[key]
 
     def match(entry: dict[Key, Any]) -> bool:
-        return all(entry[key] == value for key, value in predicate.items())
+        return all(entry[k] == v for k, v in predicate.items())
 
     base = get(base_name)
     assert isinstance(base, list)
     if accumulate:
         data = defaultdict(list)
         for entry in base:
             if not match(entry):
                 continue
-            data[make_key(entry)].append(entry)
+            index_key = make_key(entry)
+            if index_key and all(index_key):
+                data[index_key].append(entry)
         save(index_name, dict(data))
     else:
         entries = {}
         for entry in base:
             if not match(entry):
                 continue
             entries[make_key(entry)] = entry
```

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/README.md` & `schwifty-2024.5.4/schwifty/bank_registry/README.md`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_at.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_at.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_ba.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_ba.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_be.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_be.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_ch.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_ch.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_cz.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_cz.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_de.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_de.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_ee.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_ee.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_es.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_es.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_fi.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_fi.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_ge.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_ge.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_hr.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_hr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_hu.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_hu.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_it.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_it.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_kz.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_kz.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_lt.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_lt.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_lv.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_lv.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_md.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_md.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_nl.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_nl.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_no.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_no.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_pl.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_pl.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_ro.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_ro.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_rs.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_rs.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_se.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_se.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_si.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_si.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_sk.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_sk.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/generated_ua.json` & `schwifty-2024.5.4/schwifty/bank_registry/generated_ua.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_ad.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_ad.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_ae.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_ae.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_bg.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_bg.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_cr.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_cr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_cy.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_cy.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_es.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_es.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_fr.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_fr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_gb.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_gb.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_gr.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_gr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_ie.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_ie.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9567901234567903%*

 * *Differences: {'4': "{'short_name': 'Bank of Ireland'}", '8': "{'short_name': 'Citibank'}", 'delete': '[0]'}*

```diff
@@ -1,17 +1,9 @@
 [
     {
-        "bank_code": "CITI",
-        "bic": "CITIIE2XXXX",
-        "country_code": "IE",
-        "name": "Citibank Bank Europe plc",
-        "primary": true,
-        "short_name": "Citibank Bank Europe plc"
-    },
-    {
         "bank_code": "CHAS",
         "bic": "CHASIE4L",
         "country_code": "IE",
         "name": "J.P. Morgan Bank Luxembourg S.A. Dublin Branch",
         "primary": true,
         "short_name": "J.P. Morgan Bank Luxembourg S.A. Dublin Branch"
     },
@@ -41,15 +33,15 @@
     },
     {
         "bank_code": "BOFI",
         "bic": "BOFIIE2D",
         "country_code": "IE",
         "name": "Bank of Ireland Group plc",
         "primary": true,
-        "short_name": "Bank of Ireland Group plc"
+        "short_name": "Bank of Ireland"
     },
     {
         "bank_code": "BOFM",
         "bic": "BOFMIE2DXXX",
         "country_code": "IE",
         "name": "Bank of Montreal",
         "primary": true,
@@ -73,15 +65,15 @@
     },
     {
         "bank_code": "CITI",
         "bic": "CITIIE2XXXX",
         "country_code": "IE",
         "name": "Citibank Europe plc",
         "primary": true,
-        "short_name": "Citibank Europe plc"
+        "short_name": "Citibank"
     },
     {
         "bank_code": "DBIL",
         "bic": "DBILIE2DXXX",
         "country_code": "IE",
         "name": "Dell Bank International Designated Activity Company",
         "primary": true,
```

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_is.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_is.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_it.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_it.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_lu.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_lu.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_me.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_me.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_pt.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_pt.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_sa.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_sa.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/bank_registry/manual_tr.json` & `schwifty-2024.5.4/schwifty/bank_registry/manual_tr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/__init__.py` & `schwifty-2024.5.4/schwifty/checksum/__init__.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/czech_republic.py` & `schwifty-2024.5.4/schwifty/checksum/czech_republic.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/estonia.py` & `schwifty-2024.5.4/schwifty/checksum/estonia.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/france.py` & `schwifty-2024.5.4/schwifty/checksum/france.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/germany.py` & `schwifty-2024.5.4/schwifty/checksum/germany.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/iceland.py` & `schwifty-2024.5.4/schwifty/checksum/iceland.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/italy.py` & `schwifty-2024.5.4/schwifty/checksum/italy.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/netherlands.py` & `schwifty-2024.5.4/schwifty/checksum/netherlands.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/norway.py` & `schwifty-2024.5.4/schwifty/checksum/norway.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/poland.py` & `schwifty-2024.5.4/schwifty/checksum/poland.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/checksum/spain.py` & `schwifty-2024.5.4/schwifty/checksum/spain.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/iban_registry/README.md` & `schwifty-2024.5.4/schwifty/iban_registry/README.md`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/iban_registry/generated.json` & `schwifty-2024.5.4/schwifty/iban_registry/generated.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/schwifty/iban_registry/overwrite.json` & `schwifty-2024.5.4/schwifty/iban_registry/overwrite.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768192488262909%*

 * *Differences: {"'GT'": "OrderedDict([('positions', OrderedDict([('currency_code', [4, 6]), ('account_type', [6, "*

 * *         "8]), ('account_code', [8, 24])]))])",*

 * * "'MU'": "{'positions': {'currency_code': [23, 26]}, 'default_currency_code': 'MUR'}",*

 * * "'SC'": "{'positions': {'currency_code': [24, 27], delete: ['account_type']}, "*

 * *         "'default_currency_code': 'SCR'}"}*

```diff
@@ -520,14 +520,30 @@
             ],
             "national_checksum_digits": [
                 21,
                 23
             ]
         }
     },
+    "GT": {
+        "positions": {
+            "account_code": [
+                8,
+                24
+            ],
+            "account_type": [
+                6,
+                8
+            ],
+            "currency_code": [
+                4,
+                6
+            ]
+        }
+    },
     "GW": {
         "bban_length": 21,
         "bban_spec": "2!c19!n",
         "country": "GW",
         "iban_length": 25,
         "iban_spec": "GW2!n2!c19!n",
         "in_sepa_zone": false
@@ -746,18 +762,23 @@
             "national_checksum_digits": [
                 21,
                 23
             ]
         }
     },
     "MU": {
+        "default_currency_code": "MUR",
         "positions": {
             "account_code": [
                 8,
                 20
+            ],
+            "currency_code": [
+                23,
+                26
             ]
         }
     },
     "MZ": {
         "bban_length": 21,
         "bban_spec": "21!n",
         "country": "MZ",
@@ -913,20 +934,21 @@
             "national_checksum_digits": [
                 16,
                 18
             ]
         }
     },
     "SC": {
+        "default_currency_code": "SCR",
         "positions": {
             "account_code": [
                 8,
                 24
             ],
-            "account_type": [
+            "currency_code": [
                 24,
                 27
             ]
         }
     },
     "SE": {
         "positions": {
```

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_at.py` & `schwifty-2024.5.4/scripts/get_bank_registry_at.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_be.py` & `schwifty-2024.5.4/scripts/get_bank_registry_be.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_ch.py` & `schwifty-2024.5.4/scripts/get_bank_registry_ch.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_cz.py` & `schwifty-2024.5.4/scripts/get_bank_registry_cz.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_de.py` & `schwifty-2024.5.4/scripts/get_bank_registry_de.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_es.py` & `schwifty-2024.5.4/scripts/get_bank_registry_es.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_fi.py` & `schwifty-2024.5.4/scripts/get_bank_registry_fi.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_hr.py` & `schwifty-2024.5.4/scripts/get_bank_registry_hr.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_hu.py` & `schwifty-2024.5.4/scripts/get_bank_registry_hu.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_it.py` & `schwifty-2024.5.4/scripts/get_bank_registry_it.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_lt.py` & `schwifty-2024.5.4/scripts/get_bank_registry_lt.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_lv.py` & `schwifty-2024.5.4/scripts/get_bank_registry_lv.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_nl.py` & `schwifty-2024.5.4/scripts/get_bank_registry_nl.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_no.py` & `schwifty-2024.5.4/scripts/get_bank_registry_no.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_pl.py` & `schwifty-2024.5.4/scripts/get_bank_registry_pl.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_ro.py` & `schwifty-2024.5.4/scripts/get_bank_registry_ro.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_se.py` & `schwifty-2024.5.4/scripts/get_bank_registry_se.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_si.py` & `schwifty-2024.5.4/scripts/get_bank_registry_si.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_sk.py` & `schwifty-2024.5.4/scripts/get_bank_registry_sk.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_bank_registry_ua.py` & `schwifty-2024.5.4/scripts/get_bank_registry_ua.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/scripts/get_iban_registry.py` & `schwifty-2024.5.4/scripts/get_iban_registry.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/tests/test_bic.py` & `schwifty-2024.5.4/tests/test_bic.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/tests/test_checksum.py` & `schwifty-2024.5.4/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/tests/test_iban.py` & `schwifty-2024.5.4/tests/test_iban.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import pytest
 from pycountry import countries  # type: ignore
 
 from schwifty import IBAN
 from schwifty.exceptions import SchwiftyException
+from schwifty.iban import convert_bban_spec_to_regex
 
 
 valid = [
     "AL47 2121 1009 0000 0002 3569 8741",  # Albania
     "AD12 0001 2030 2003 5910 0100",  # Andorra
     "AT61 1904 3002 3457 3201",  # Austria
     "AZ21 NABZ 0000 0000 1370 1000 1944",  # Republic of Azerbaijan
@@ -361,14 +362,25 @@
 
 def test_random_iban() -> None:
     for _ in range(100):
         iban = IBAN.random()
         assert isinstance(iban, IBAN)
 
 
+def test_random_special_cases() -> None:
+    iban = IBAN.random(country_code="MU")
+    assert iban.endswith("000MUR")
+
+    iban = IBAN.random(country_code="SC")
+    assert iban.endswith("SCR")
+
+    iban = IBAN.random(country_code="KM")
+    assert iban.is_valid
+
+
 def test_pydantic_protocol() -> None:
     from pydantic import BaseModel
     from pydantic import ValidationError
 
     class Model(BaseModel):
         iban: IBAN
 
@@ -388,7 +400,22 @@
     assert json_schema["properties"]["iban"] == {"maxLength": 34, "title": "IBAN", "type": "string"}
 
     dumped = model.model_dump_json()
     assert dumped == '{"iban":"GL8964710001000206"}'
 
     loaded = Model.model_validate_json(dumped)
     assert loaded == model
+
+
+@pytest.mark.parametrize(
+    ("spec", "regex"),
+    [
+        ("5!n", r"^\d{5}$"),
+        ("4!a", r"^[A-Z]{4}$"),
+        ("10!c", r"^[A-Za-z0-9]{10}$"),
+        ("5!e", r"^ {5}$"),
+        ("3n", r"^\d{1,3}$"),
+        ("5!n3!a", r"^\d{5}[A-Z]{3}$"),
+    ],
+)
+def test_convert_bban_spec_to_regex(spec: str, regex: str) -> None:
+    assert convert_bban_spec_to_regex(spec) == regex
```

### Comparing `schwifty-2024.5.3/tests/test_registry.py` & `schwifty-2024.5.4/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/LICENSE` & `schwifty-2024.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/README.rst` & `schwifty-2024.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/hatch.toml` & `schwifty-2024.5.4/hatch.toml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/pyproject.toml` & `schwifty-2024.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.3/PKG-INFO` & `schwifty-2024.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: schwifty
-Version: 2024.5.3
+Version: 2024.5.4
 Project-URL: Changelog, https://github.com/mdomke/schwifty/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://schwifty.readthedocs.io/en/latest/
 Project-URL: Homepage, http://github.com/mdomke/schwifty
 Author-email: Martin Domke <mail@martindomke.net>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

