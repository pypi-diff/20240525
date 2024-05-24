# Comparing `tmp/extended_mypy_django_plugin-0.5.2.tar.gz` & `tmp/extended_mypy_django_plugin-0.5.3.tar.gz`

## Comparing `extended_mypy_django_plugin-0.5.2.tar` & `extended_mypy_django_plugin-0.5.3.tar`

### file list

```diff
@@ -1,99 +1,112 @@
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.readthedocs.yaml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/DEVELOPMENT.rst
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/find
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/format
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/lint
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/mypy.ini
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/pytest.ini
--rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/run.sh
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/test.sh
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tox.ini
--rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/types
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.github/workflows/ciold.yml
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.github/workflows/lintold.yml
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.github/workflows/release.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/.gitignore
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/README.rst
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/conf.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/index.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/_static/css/extra.css
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/changelog.rst
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/installation.rst
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/primer.rst
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/tracking-changes.rst
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/usage.rst
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/actions.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/config.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/dependencies.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/hook.rst
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/index.rst
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/plugin.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/reports.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/docs/api/internals/store.rst
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/manage.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/mypy.ini
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/asgi.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/settings.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/urls.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/version.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/views.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp/apps.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp2/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp2/apps.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp2/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp2/migrations/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/__init__.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/annotations.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/entry.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/py.typed
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/version.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/__init__.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_config.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_debug.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_dependencies.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_hook.py
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_plugin.py
--rw-r--r--   0        0        0    15489 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_reports.py
--rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_store.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/__init__.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_type_analyze.py
--rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_type_checker.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/scripts/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/scripts/determine_django_state.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/scripts/find_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/make_old.patch
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/py.typed
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/test_settings.py
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/tests_extension_hook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp/apps.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp2/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp2/apps.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/scripts/myapp2/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tests/test_concrete_annotation.yml
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tests/test_works.yml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/.gitignore
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/bootstrap_venvstarter.py
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/devtools.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/requirements.dev.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/requirements.docs.txt
--rwxr-xr-x   0        0        0     1108 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/tools/venv
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/LICENSE
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/README.rst
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/DEVELOPMENT.rst
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/find
+-rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/format
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/lint
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/mypy.ini
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/pytest.ini
+-rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/run.sh
+-rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/test.sh
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/tox.ini
+-rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/types
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/.github/workflows/ciold.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/.github/workflows/lintold.yml
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/.gitignore
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/README.rst
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/conf.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/index.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/_static/css/extra.css
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/changelog.rst
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/installation.rst
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/primer.rst
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/tracking-changes.rst
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/usage.rst
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/internals/actions.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/internals/config.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/internals/dependencies.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/internals/hook.rst
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/internals/index.rst
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/internals/plugin.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/internals/reports.rst
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/docs/api/internals/store.rst
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/manage.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/mypy.ini
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/asgi.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/settings.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/urls.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/version.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/views.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/exampleapp/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/exampleapp/apps.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/exampleapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/exampleapp/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/exampleapp2/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/exampleapp2/apps.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/exampleapp2/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/example/djangoexample/exampleapp2/migrations/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/__init__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/annotations.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/entry.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/py.typed
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/version.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/__init__.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_config.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_debug.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_dependencies.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_helpers.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_hook.py
+-rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_plugin.py
+-rw-r--r--   0        0        0    15865 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_reports.py
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_store.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/actions/__init__.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/actions/_type_analyze.py
+-rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/actions/_type_checker.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/scripts/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/scripts/determine_django_state.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/scripts/find_models.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/make_old.patch
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/follower1/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/follower1/apps.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/follower1/models/__init__.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/follower1/models/follower1.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/leader/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/leader/apps.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/leader/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/myapp/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/myapp/apps.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/myapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/myapp2/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/myapp2/apps.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/myapp2/models.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/test_helpers/pyproject.toml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/test_helpers/extended_mypy_django_plugin_test_driver/__init__.py
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/test_helpers/extended_mypy_django_plugin_test_driver/extension_hook.py
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/test_helpers/extended_mypy_django_plugin_test_driver/output_builder.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/test_helpers/extended_mypy_django_plugin_test_driver/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/test_helpers/extended_mypy_django_plugin_test_driver/py.typed
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/test_helpers/extended_mypy_django_plugin_test_driver/scenario.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/test_helpers/extended_mypy_django_plugin_test_driver/settings.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/scripts/test_helpers/extended_mypy_django_plugin_test_driver/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0    17070 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/tests/test_concrete_annotations.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/tests/test_works.yml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/tools/.gitignore
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/tools/bootstrap_venvstarter.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/tools/devtools.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/tools/requirements.dev.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/tools/requirements.docs.txt
+-rwxr-xr-x   0        0        0     1326 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/tools/venv
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/README.rst
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.3/PKG-INFO
```

### Comparing `extended_mypy_django_plugin-0.5.2/DEVELOPMENT.rst` & `extended_mypy_django_plugin-0.5.3/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/run.sh` & `extended_mypy_django_plugin-0.5.3/run.sh`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/.github/workflows/ci.yml` & `extended_mypy_django_plugin-0.5.3/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 ---
 
 name: CI tasks
 
-on: [push, pull_request]
+on:
+  pull_request: {}
+  push:
+    branches:
+      - main
+
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
 
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
```

### Comparing `extended_mypy_django_plugin-0.5.2/.github/workflows/ciold.yml` & `extended_mypy_django_plugin-0.5.3/.github/workflows/ciold.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 ---
 
 name: CI tasks for old versions
 
-on: [push, pull_request]
+on:
+  pull_request: {}
+  push:
+    branches:
+      - main
+
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
 
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
```

### Comparing `extended_mypy_django_plugin-0.5.2/.github/workflows/lint.yml` & `extended_mypy_django_plugin-0.5.3/.github/workflows/lintold.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,64 @@
 ---
 
-name: Lint
+name: Lint for old versions
 
-on: [push, pull_request]
+on:
+  pull_request: {}
+  push:
+    branches:
+      - main
+
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
+      - name: Install patch to make this use old versions of things
+        run: |
+          git config user.name github-actions
+          git config user.email github-actions@github.com
+          git am ./scripts/make_old.patch
+
       - name: Install deps
         shell: bash
         env:
           VENVSTARTER_ONLY_MAKE_VENV: "1"
         run: python ./tools/venv
 
       - name: Ensure linter is happy
         run: ./lint
 
   types:
     runs-on: ubuntu-latest
-    strategy:
-      fail-fast: false
-      matrix:
-        python-version: ["3.10", "3.11", "3.12"]
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python-version }}
+          python-version: "3.10"
+
+      - name: Install patch to make this use old versions of things
+        run: |
+          git config user.name github-actions
+          git config user.email github-actions@github.com
+          git am ./scripts/make_old.patch
 
       - name: Install deps
         shell: bash
         env:
           VENVSTARTER_ONLY_MAKE_VENV: "1"
         run: python ./tools/venv
 
       - name: Ensure mypy is happy
         run: ./types
-
-  format:
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.10"
-
-      - name: Install deps
-        shell: bash
-        env:
-          VENVSTARTER_ONLY_MAKE_VENV: "1"
-        run: python ./tools/venv
-
-      - name: Ensure code is formatted
-        run: |
-          ./format
-
-          # Complain if there were changes
-          if [[ ! -z "$(git status --porcelain)" ]]; then
-            echo "=========================================="
-            echo "Found changes!"
-            echo "Please run ./format before committing code"
-            echo "=========================================="
-            git diff
-            exit 1
-          fi
```

### Comparing `extended_mypy_django_plugin-0.5.2/.github/workflows/release.yml` & `extended_mypy_django_plugin-0.5.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/docs/conf.py` & `extended_mypy_django_plugin-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/docs/api/changelog.rst` & `extended_mypy_django_plugin-0.5.3/docs/api/changelog.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 .. _changelog:
 
 Changelog
 ---------
 
+.. _release-0.5.3:
+
+0.5.3 - 25 May 2024
+    * Resolve Invalid cross-device link error when default temporary folder
+      is on a different device to the scratch path.
+    * Add a fix for a weird corner case in django-stubs where a certain pattern
+      of changes after a previous dmypy run would crash dmypy
+
 .. _release-0.5.2:
 
 0.5.2 - 22 May 2024
     * Add more confidence get_function_hook doesn't steal from django-stubs
 
 .. _release-0.5.1:
```

### Comparing `extended_mypy_django_plugin-0.5.2/docs/api/installation.rst` & `extended_mypy_django_plugin-0.5.3/docs/api/installation.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/docs/api/primer.rst` & `extended_mypy_django_plugin-0.5.3/docs/api/primer.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/docs/api/tracking-changes.rst` & `extended_mypy_django_plugin-0.5.3/docs/api/tracking-changes.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/docs/api/usage.rst` & `extended_mypy_django_plugin-0.5.3/docs/api/usage.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/docs/api/internals/actions.rst` & `extended_mypy_django_plugin-0.5.3/docs/api/internals/actions.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/example/manage.py` & `extended_mypy_django_plugin-0.5.3/example/manage.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/example/djangoexample/settings.py` & `extended_mypy_django_plugin-0.5.3/example/djangoexample/settings.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/example/djangoexample/urls.py` & `extended_mypy_django_plugin-0.5.3/example/djangoexample/urls.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/example/djangoexample/views.py` & `extended_mypy_django_plugin-0.5.3/example/djangoexample/views.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/example/djangoexample/exampleapp/models.py` & `extended_mypy_django_plugin-0.5.3/example/djangoexample/exampleapp/models.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/annotations.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/annotations.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/entry.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/entry.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_config.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_config.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_dependencies.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_dependencies.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_hook.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_hook.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_plugin.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import collections
 import enum
 import sys
 from typing import Generic
 
 from mypy.checker import TypeChecker
 from mypy.modulefinder import mypy_path
 from mypy.nodes import MypyFile, TypeInfo
 from mypy.options import Options
 from mypy.plugin import (
     AnalyzeTypeContext,
     AttributeContext,
+    ClassDefContext,
     DynamicClassDefContext,
     FunctionContext,
 )
 from mypy.semanal import SemanticAnalyzer
 from mypy.typeanal import TypeAnalyser
 from mypy.types import CallableType, Instance
 from mypy.types import Type as MypyType
@@ -20,15 +22,15 @@
 from mypy_django_plugin.django.context import DjangoContext
 from mypy_django_plugin.transformers.managers import (
     resolve_manager_method,
     resolve_manager_method_from_instance,
 )
 from typing_extensions import assert_never
 
-from . import _config, _dependencies, _hook, _reports, _store, actions
+from . import _config, _dependencies, _helpers, _hook, _reports, _store, actions
 
 
 class Hook(
     Generic[_hook.T_Ctx, _hook.T_Ret],
     _hook.Hook["ExtendedMypyStubs", _hook.T_Ctx, _hook.T_Ret],
 ):
     store: _store.Store
@@ -43,14 +45,16 @@
     ``mypy_django_plugin.main.NewSemanalDjangoPlugin`` found in the active python
     environment.
 
     It implements the following mypy plugin hooks:
 
     .. automethod:: get_additional_deps
 
+    .. autoattribute:: get_base_class_hook
+
     .. autoattribute:: get_dynamic_class_hook
 
     .. autoattribute:: get_type_analyze_hook
 
     .. autoattribute:: get_function_hook
 
     .. autoattribute:: get_attribute_hook
@@ -70,21 +74,25 @@
         self.plugin_config = _config.Config(options.config_file)
         # Add paths from MYPYPATH env var
         sys.path.extend(mypy_path())
         # Add paths from mypy_path config option
         sys.path.extend(options.mypy_path)
 
         self.running_in_daemon: bool = "dmypy" in sys.argv[0]
+
+        # Ensure we have a working django context before doing anything
+        # So when we try to import things that depend on that, they don't crash us!
+        self.django_context = DjangoContext(self.plugin_config.django_settings_module)
+
         self.report = _reports.Reports.create(
             determine_django_state_script=self.plugin_config.determine_django_state_script,
             django_settings_module=self.plugin_config.django_settings_module,
             scratch_path=self.plugin_config.scratch_path,
         )
 
-        self.django_context = DjangoContext(self.plugin_config.django_settings_module)
         self.store = _store.Store(
             get_model_class_by_fullname=self.django_context.get_model_class_by_fullname,
             lookup_info=self._lookup_info,
             django_context_model_modules=self.django_context.model_modules,
             is_installed_model=self._is_installed_model,
             known_concrete_models=self.report.known_concrete_models,
         )
@@ -132,14 +140,73 @@
         """
         results = self.dependencies.for_file(
             file.fullname, imports=file.imports, super_deps=super().get_additional_deps(file)
         )
         return results
 
     @_hook.hook
+    class get_base_class_hook(Hook[ClassDefContext, None]):
+        """
+        We need to make up for a bug in django-stubs
+        """
+
+        def choose(self) -> bool:
+            if self.super_hook is None:
+                return False
+
+            if _helpers.get_is_abstract_model() is None:
+                return False
+
+            sym = self.plugin.lookup_fully_qualified(self.fullname)
+            return bool(
+                sym is not None
+                and isinstance(sym.node, TypeInfo)
+                and _helpers.is_model_type(sym.node)
+            )
+
+        def run(self, ctx: ClassDefContext) -> None:
+            if self.super_hook is None:
+                return None
+
+            # Copy the code in django-stubs that crashes
+            # And fill in the missing information before continuing
+            processed_models = set()
+            model_bases = collections.deque([ctx.cls])
+            while model_bases:
+                model = model_bases.popleft()
+
+                try:
+                    # Whether this causes an AssertionError or an AttributeError depends
+                    # on whether mypy is compiled or not
+                    # Note that this only appears to trigger on followup changes with a cache
+                    # in very specific situations
+                    for base in model.info.bases:
+                        break
+                except AssertionError as exc:
+                    if str(exc) == "ClassDef is lacking info":
+                        sym = self.plugin.lookup_fully_qualified(model.fullname)
+                        if sym and isinstance(sym.node, TypeInfo):
+                            model.info = sym.node
+                except AttributeError as exc:
+                    if str(exc) == "attribute 'bases' of 'TypeInfo' undefined":
+                        sym = self.plugin.lookup_fully_qualified(model.fullname)
+                        if sym and isinstance(sym.node, TypeInfo):
+                            model.info = sym.node
+
+                for base in model.info.bases:
+                    if (
+                        _helpers.is_abstract_model(base.type)
+                        and base.type.fullname not in processed_models
+                    ):
+                        model_bases.append(base.type.defn)
+                        processed_models.add(base.type.fullname)
+
+            return self.super_hook(ctx)
+
+    @_hook.hook
     class get_dynamic_class_hook(Hook[DynamicClassDefContext, None]):
         """
         This is used to find ``Concrete.type_var`` and turn that into a ``TypeVar``
         representing each Concrete class of the abstract model provided.
 
         So say we find::
```

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_reports.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_reports.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import importlib.resources
 import importlib.util
 import io
 import itertools
 import pathlib
 import re
 import shlex
+import shutil
 import stat
 import subprocess
 import sys
 import tempfile
 import textwrap
 import time
 import zlib
@@ -59,14 +60,18 @@
         if not reports_dir.exists():
             reports_dir.mkdir(parents=True, exist_ok=True)
 
         for path in reports_dir.iterdir():
             mod: str | None = None
             summary: str | None = None
 
+            if path.is_dir():
+                shutil.rmtree(path)
+                continue
+
             if path.suffix == ".py":
                 for line in path.read_text().splitlines():
                     m = regexes["mod_decl"].match(line)
                     if m:
                         mod = m.groupdict()["mod"]
 
                     m = regexes["summary_decl"].match(line)
@@ -114,15 +119,15 @@
                     break
 
         if summary != previous_summary:
             (directory / f"{name}.py").write_text(content)
         return name
 
     def add_mod(self, mod: str) -> str:
-        with tempfile.TemporaryDirectory() as tmp:
+        with tempfile.TemporaryDirectory(dir=self.reports_dir, prefix=".tmp") as tmp:
             temp_dir = pathlib.Path(tmp)
             summary = f"{mod} ||>"
             name = self._write_mod(temp_dir, mod, summary, empty=True)
             made = temp_dir / f"{name}.py"
             if made.exists():
                 made.rename(self.reports_dir / f"{name}.py")
             return f"{self.prefix}.{name}"
@@ -133,15 +138,15 @@
             modules=modules,
             reports_dir=self.reports_dir,
             modules_to_report_name=self.modules_to_report_name,
         )
 
         # Prevent partial writes by dumping to a temp directory and moving changed files
         # We also don't simply rename the entire directory so unchanged files remain unchanged
-        with tempfile.TemporaryDirectory() as tmp:
+        with tempfile.TemporaryDirectory(dir=self.reports_dir, prefix=".tmp") as tmp:
             temp_dir = pathlib.Path(tmp)
             for mod, summary in instance.modules.items():
                 instance._write_mod(temp_dir, mod, summary)
 
             for path in temp_dir.iterdir():
                 destination = instance.reports_dir / path.name
                 if not destination.exists():
@@ -304,14 +309,20 @@
 
     def known_concrete_models(self, fullname: str) -> set[str]:
         return self._known_concrete_models[fullname]
 
     def lines_hash(self) -> str:
         buffer = io.BytesIO()
         for path in self._store.reports_dir.iterdir():
+            valid_dependency = (
+                path.is_file() and path.suffix == ".py" and not path.name.startswith(".")
+            )
+            if not valid_dependency:
+                continue
+
             content = path.read_bytes()
             if b"def value_not_installed" not in content:
                 buffer.write(b"\n")
                 buffer.write(path.name.encode())
                 buffer.write(b"\n")
                 buffer.write(path.read_bytes())
```

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/_store.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/_store.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_type_analyze.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/actions/_type_analyze.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/plugin/actions/_type_checker.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/plugin/actions/_type_checker.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/scripts/determine_django_state.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/scripts/determine_django_state.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/extended_mypy_django_plugin/scripts/find_models.py` & `extended_mypy_django_plugin-0.5.3/extended_mypy_django_plugin/scripts/find_models.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/scripts/make_old.patch` & `extended_mypy_django_plugin-0.5.3/scripts/make_old.patch`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 index b84fdfa..1bbec65 100755
 --- a/tools/venv
 +++ b/tools/venv
 @@ -19,7 +19,7 @@ manager.add_local_dep(
      "{here}",
      "..",
      version_file=("extended_mypy_django_plugin", "version.py"),
--    name="extended_mypy_django_plugin[stubs-latest,tests]=={version}",
-+    name="extended_mypy_django_plugin[stubs-older,tests]=={version}",
+-    name="extended_mypy_django_plugin[stubs-latest]=={version}",
++    name="extended_mypy_django_plugin[stubs-older]=={version}",
  )
  
  manager.add_local_dep(
 -- 
 2.44.0
```

### Comparing `extended_mypy_django_plugin-0.5.2/scripts/tests_extension_hook.py` & `extended_mypy_django_plugin-0.5.3/scripts/test_helpers/extended_mypy_django_plugin_test_driver/extension_hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import ast
-import dataclasses
 import os
 import pathlib
 import runpy
 from collections.abc import Mapping, MutableSequence
 from typing import TYPE_CHECKING
 
 from pytest_mypy_plugins import (
@@ -13,15 +12,15 @@
     MypyPluginsScenario,
     OutputMatcher,
     ScenarioHookMaker,
     ScenarioHooks,
     ScenarioHooksRunAndCheckOptions,
 )
 
-here = pathlib.Path(__file__).parent
+scripts_dir = pathlib.Path(__file__).parent.parent.parent
 
 
 def django_plugin_hook(item: ItemForHook) -> None:
     django_settings_section = (
         "\n[mypy.plugins.django-stubs]\n" "django_settings_module = mysettings"
     )
 
@@ -43,16 +42,14 @@
         additional_properties: Mapping[str, object],
     ) -> ScenarioHooksRunAndCheckOptions:
         custom_settings = additional_properties.get("custom_settings", None)
         copied_apps = additional_properties.get("copied_apps", None)
         installed_apps = additional_properties.get("installed_apps", None)
         monkeypatch = additional_properties.get("monkeypatch", None)
 
-        options = dataclasses.replace(options, start=["."])
-
         if "debug" in additional_properties:
             pathlib.Path("/tmp/debug").write_text("")
         else:
             pathlib.Path("/tmp/debug").unlink(missing_ok=True)
 
         if isinstance(copied_apps, list):
             for app in copied_apps:
@@ -137,24 +134,27 @@
         settings_values = runpy.run_path(str(current_settings))
         installed_apps = settings_values["INSTALLED_APPS"]
 
         if not isinstance(installed_apps, list):
             installed_apps = []
 
         for app in installed_apps:
-            if (here / app).exists():
+            if (scripts_dir / app).exists():
                 self._copy_app(scenario, app)
 
         return options
 
     def _copy_app(self, scenario: MypyPluginsScenario, app: str) -> None:
-        for root, _, files in os.walk(here / app):
+        for root, _, files in os.walk(scripts_dir / app):
             for name in files:
+                if name.endswith(".pyc"):
+                    continue
+
                 location = pathlib.Path(root, name)
-                path = location.relative_to(here)
+                path = location.relative_to(scripts_dir)
                 if not (pathlib.Path.cwd() / path).exists():
                     scenario.handle_followup_file(
                         FollowupFile(path=str(path), content=location.read_text())
                     )
 
 
 if TYPE_CHECKING:
```

### Comparing `extended_mypy_django_plugin-0.5.2/scripts/myapp/models.py` & `extended_mypy_django_plugin-0.5.3/scripts/myapp/models.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/tests/test_works.yml` & `extended_mypy_django_plugin-0.5.3/tests/test_works.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 - case: mypy_path_from_env
+  start: .
   disable_cache: true
   out: |
      main:33: note: Revealed type is "Union[django.db.models.manager.Manager[myapp.models.Child1], myapp.models.ManagerFromChild2QuerySet[myapp.models.Child2], django.db.models.manager.Manager[myapp.models.Child3], django.db.models.manager.Manager[myapp2.models.ChildOther]]"
      main:38: note: Revealed type is "myapp.models.Child1"
      main:41: note: Revealed type is "Union[django.db.models.query._QuerySet[myapp.models.Child1, myapp.models.Child1], myapp.models.Child2QuerySet, django.db.models.query._QuerySet[myapp.models.Child3, myapp.models.Child3], django.db.models.query._QuerySet[myapp2.models.ChildOther, myapp2.models.ChildOther]]"
      main:44: note: Revealed type is "django.db.models.query._QuerySet[myapp.models.Child1, myapp.models.Child1]"
      main:47: note: Revealed type is "myapp.models.Child2QuerySet"
```

### Comparing `extended_mypy_django_plugin-0.5.2/tools/bootstrap_venvstarter.py` & `extended_mypy_django_plugin-0.5.3/tools/bootstrap_venvstarter.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/tools/devtools.py` & `extended_mypy_django_plugin-0.5.3/tools/devtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             example_root = here.parent / "example"
             if any(path.is_relative_to(example_root) for path in paths):
                 if not all(path.is_relative_to(example_root) for path in paths):
                     raise ValueError("If specifying an example path, all paths must be from there")
                 os.chdir(example_root)
             locations = [str(path) for path in paths]
 
-        run(bin_dir / "mypy", *locations, *args)
+        run(bin_dir / "mypy", *locations, *args, "--enable-incomplete-feature=Unpack")
 
         if not specified:
             os.chdir(here.parent / "example")
             run(bin_dir / "mypy", ".", *args)
 
     @command
     def tests(self, bin_dir: Path, args: list[str]) -> None:
```

### Comparing `extended_mypy_django_plugin-0.5.2/LICENSE` & `extended_mypy_django_plugin-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/README.rst` & `extended_mypy_django_plugin-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5.2/pyproject.toml` & `extended_mypy_django_plugin-0.5.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 readme = "README.rst"
 license = { text = "MIT" }
 authors = [
     { name = "Stephen Moore", email = "stephen@delfick.com" },
 ]
 
 [project.optional-dependencies]
-tests = [
-    "pytest==8.1.1",
-]
 stubs-latest = [
     "mypy==1.10.0",
     "django-stubs==5.0.0",
 ]
 stubs-older = [
     "mypy==1.4.0",
     "django-stubs==4.2.3",
```

### Comparing `extended_mypy_django_plugin-0.5.2/PKG-INFO` & `extended_mypy_django_plugin-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.3
 Name: extended-mypy-django-plugin
-Version: 0.5.2
+Version: 0.5.3
 Summary: Trying to make mypy understand .objects on abstract django models
 Author-email: Stephen Moore <stephen@delfick.com>
 License: MIT
 License-File: LICENSE
 Provides-Extra: stubs-latest
 Requires-Dist: django-stubs==5.0.0; extra == 'stubs-latest'
 Requires-Dist: mypy==1.10.0; extra == 'stubs-latest'
 Provides-Extra: stubs-older
 Requires-Dist: django-stubs==4.2.3; extra == 'stubs-older'
 Requires-Dist: mypy==1.4.0; extra == 'stubs-older'
-Provides-Extra: tests
-Requires-Dist: pytest==8.1.1; extra == 'tests'
 Description-Content-Type: text/x-rst
 
 Extended ``django-stubs``
 =========================
 
 This is an extension on the `django-stubs`_ project that attempts to make it
 possible to work with abstract Django ORM models as if they represent all the
```

