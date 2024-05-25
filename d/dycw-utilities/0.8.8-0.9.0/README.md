# Comparing `tmp/dycw_utilities-0.8.8.tar.gz` & `tmp/dycw_utilities-0.9.0.tar.gz`

## Comparing `dycw_utilities-0.8.8.tar` & `dycw_utilities-0.9.0.tar`

### file list

```diff
@@ -1,222 +1,222 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.envrc
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.rgiginore
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/Makefile
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/conftest.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/noxfile.py
--rw-r--r--   0        0        0     8883 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/requirements-dev.txt
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.github/workflows/push.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/conftest.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_airium.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_atomicwrites.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_beartype.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_bidict.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_class_name.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_clean_dir.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_cryptography.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_cvxpy.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_datetime.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_email.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_enum.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_errors.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_fastapi.py
--rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_fastparquet.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_fpdf2.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_getpass.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_git.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_hashlib.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_hatch.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_iterables.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_json.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_logging.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_memory_profiler.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_modules.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_monitor_memory.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_more_itertools.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_os.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pathlib.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pickle.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pqdm.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pyinstrument.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pypi_server.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pytest.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_pytest_check.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_random.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_re.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_scipy.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_semver.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_sentinel.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_socket.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_subprocess.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_sys.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_tempfile.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_text.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_timer.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_tqdm.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_typed_settings.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_types.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_typing.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_warnings.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_zipfile.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/test_zoneinfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/attrs/__init__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/attrs/test_attrs.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/attrs/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/click/__init__.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/click/test_click.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/click/test_luigi.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/click/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/holoviews/__init__.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/holoviews/test_holoviews.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/holoviews/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_hypothesis.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_luigi.py
--rw-r--r--   0        0        0    17438 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_numpy.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_pandas.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_semver.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_sqlalchemy.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/hypothesis/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/loguru/__init__.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/loguru/script_to_test_luigi.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/loguru/test_loguru.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/__init__.py
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/test_attrs.py
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/test_luigi.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/test_semver.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/test_server.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/luigi/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/math/__init__.py
--rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/math/test_math.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/math/test_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/standalone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/outer_1.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/outer_2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/subpackage/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/subpackage/inner_1.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/subpackage/inner_2.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_with/subpackage/inner_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_without/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_without/module_1.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/modules/package_without/module_2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/numpy/__init__.py
--rw-r--r--   0        0        0    45851 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/numpy/test_numpy.py
--rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/numpy/test_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/pandas/__init__.py
--rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/pandas/test_pandas.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/pandas/test_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/sqlalchemy/test_fastparquet.py
--rw-r--r--   0        0        0    14095 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/sqlalchemy/test_pandas.py
--rw-r--r--   0        0        0    38826 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/sqlalchemy/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/xarray/__init__.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/xarray/test_typing.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/xarray/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/zarr/__init__.py
--rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/zarr/test_xarray.py
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/tests/zarr/test_zarr.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/airium.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/atomicwrites.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/beartype.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/bidict.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/class_name.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/cryptography.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/cvxpy.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/datetime.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/email.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/enum.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/errors.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/fastapi.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/fastparquet.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/fpdf2.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/getpass.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/git.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hashlib.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hatch.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/iterables.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/json.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/logging.py
--rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/loguru.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/memory_profiler.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/modules.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/more_itertools.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/os.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pathlib.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pickle.py
--rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pqdm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/py.typed
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pyinstrument.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pytest.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pytest_check.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/random.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/re.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/scipy.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/semver.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/sentinel.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/socket.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/subprocess.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/sys.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/tempfile.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/text.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/timer.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/tqdm.py
--rw-r--r--   0        0        0     6505 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/typed_settings.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/types.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/typing.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/warnings.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/zipfile.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/zoneinfo.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/attrs/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/attrs/xarray.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/clean_dir/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/clean_dir/__main__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/clean_dir/classes.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/click/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/click/luigi.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/click/sqlalchemy.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/holoviews/__init__.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/holoviews/xarray.py
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/luigi.py
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/numpy.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/pandas.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/semver.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/sqlalchemy.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/typing.py
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/hypothesis/xarray.py
--rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/__init__.py
--rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/attrs.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/semver.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/sqlalchemy.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/server/__init__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/server/__main__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/luigi/server/classes.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/math/__init__.py
--rw-r--r--   0        0        0    14378 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/math/typing.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/monitor_memory/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/monitor_memory/__main__.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/monitor_memory/classes.py
--rw-r--r--   0        0        0    17896 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/numpy/__init__.py
--rw-r--r--   0        0        0    32371 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/numpy/typing.py
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pandas/__init__.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pandas/typing.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pypi_server/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pypi_server/__main__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/pypi_server/classes.py
--rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/sqlalchemy/fastparquet.py
--rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/sqlalchemy/pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/xarray/__init__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/xarray/typing.py
--rw-r--r--   0        0        0    10192 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/zarr/__init__.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/utilities/zarr/xarray.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/.gitignore
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/README.md
--rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 dycw_utilities-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/.envrc
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/.rgiginore
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/Makefile
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/conftest.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/noxfile.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/requirements-dev.txt
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/.github/workflows/push.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_airium.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_atomicwrites.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_beartype.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_bidict.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_class_name.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_clean_dir.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_cryptography.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_cvxpy.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_datetime.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_email.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_enum.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_errors.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_fastapi.py
+-rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_fastparquet.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_fpdf2.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_getpass.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_git.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_hashlib.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_hatch.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_iterables.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_json.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_logging.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_memory_profiler.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_modules.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_monitor_memory.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_more_itertools.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_os.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_pathlib.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_pickle.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_pqdm.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_pyinstrument.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_pypi_server.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_pytest.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_pytest_check.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_random.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_re.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_scipy.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_semver.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_sentinel.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_socket.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_subprocess.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_sys.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_tempfile.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_text.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_timer.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_tqdm.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_typed_settings.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_types.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_typing.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_warnings.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_zipfile.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/test_zoneinfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/attrs/__init__.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/attrs/test_attrs.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/attrs/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/click/__init__.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/click/test_click.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/click/test_luigi.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/click/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/holoviews/__init__.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/holoviews/test_holoviews.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/holoviews/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/hypothesis/test_hypothesis.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/hypothesis/test_luigi.py
+-rw-r--r--   0        0        0    17438 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/hypothesis/test_numpy.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/hypothesis/test_pandas.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/hypothesis/test_semver.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/hypothesis/test_sqlalchemy.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/hypothesis/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/loguru/__init__.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/loguru/script_to_test_luigi.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/loguru/test_loguru.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/luigi/__init__.py
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/luigi/test_attrs.py
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/luigi/test_luigi.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/luigi/test_semver.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/luigi/test_server.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/luigi/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/math/__init__.py
+-rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/math/test_math.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/math/test_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/standalone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/package_with/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/package_with/outer_1.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/package_with/outer_2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/package_with/subpackage/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/package_with/subpackage/inner_1.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/package_with/subpackage/inner_2.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/package_with/subpackage/inner_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/package_without/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/package_without/module_1.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/modules/package_without/module_2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/numpy/__init__.py
+-rw-r--r--   0        0        0    45851 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/numpy/test_numpy.py
+-rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/numpy/test_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/pandas/__init__.py
+-rw-r--r--   0        0        0    10976 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/pandas/test_pandas.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/pandas/test_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/sqlalchemy/test_fastparquet.py
+-rw-r--r--   0        0        0    14095 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/sqlalchemy/test_pandas.py
+-rw-r--r--   0        0        0    38826 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/sqlalchemy/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/xarray/__init__.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/xarray/test_typing.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/xarray/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/zarr/__init__.py
+-rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/zarr/test_xarray.py
+-rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/tests/zarr/test_zarr.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/airium.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/atomicwrites.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/beartype.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/bidict.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/class_name.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/cryptography.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/cvxpy.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/datetime.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/email.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/enum.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/errors.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/fastapi.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/fastparquet.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/fpdf2.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/getpass.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/git.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/hashlib.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/hatch.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/iterables.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/json.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/logging.py
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/loguru.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/memory_profiler.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/modules.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/more_itertools.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/os.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pathlib.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pickle.py
+-rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pqdm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/py.typed
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pyinstrument.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pytest.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pytest_check.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/random.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/re.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/scipy.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/semver.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/sentinel.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/socket.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/subprocess.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/sys.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/tempfile.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/text.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/timer.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/tqdm.py
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/typed_settings.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/types.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/typing.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/warnings.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/zipfile.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/zoneinfo.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/attrs/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/attrs/xarray.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/clean_dir/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/clean_dir/__main__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/clean_dir/classes.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/click/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/click/luigi.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/click/sqlalchemy.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/holoviews/__init__.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/holoviews/xarray.py
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/hypothesis/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/hypothesis/luigi.py
+-rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/hypothesis/numpy.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/hypothesis/pandas.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/hypothesis/semver.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/hypothesis/sqlalchemy.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/hypothesis/typing.py
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/hypothesis/xarray.py
+-rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/luigi/__init__.py
+-rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/luigi/attrs.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/luigi/semver.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/luigi/sqlalchemy.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/luigi/server/__init__.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/luigi/server/__main__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/luigi/server/classes.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/math/__init__.py
+-rw-r--r--   0        0        0    14378 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/math/typing.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/monitor_memory/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/monitor_memory/__main__.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/monitor_memory/classes.py
+-rw-r--r--   0        0        0    17896 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/numpy/__init__.py
+-rw-r--r--   0        0        0    32371 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/numpy/typing.py
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pandas/__init__.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pandas/typing.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pypi_server/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pypi_server/__main__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/pypi_server/classes.py
+-rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/sqlalchemy/fastparquet.py
+-rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/xarray/__init__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/xarray/typing.py
+-rw-r--r--   0        0        0    10192 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/zarr/__init__.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/utilities/zarr/xarray.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/README.md
+-rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 dycw_utilities-0.9.0/PKG-INFO
```

### Comparing `dycw_utilities-0.8.8/.pre-commit-config.yaml` & `dycw_utilities-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/noxfile.py` & `dycw_utilities-0.9.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/requirements-dev.txt` & `dycw_utilities-0.9.0/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # via
     #   cattrs
     #   dycw-utilities (pyproject.toml)
     #   hypothesis
     #   outcome
     #   trio
     #   typed-settings
-beartype==0.13.0
+beartype==0.13.1
     # via dycw-utilities (pyproject.toml)
 bidict==0.22.1
     # via dycw-utilities (pyproject.toml)
 black==23.3.0
     # via dycw-utilities (pyproject.toml)
 bleach==6.0.0
     # via panel
@@ -70,15 +70,15 @@
     # via
     #   coverage-conditional-plugin
     #   pytest-cov
 coverage-conditional-plugin==0.8.0
     # via dycw-utilities (pyproject.toml)
 cramjam==2.6.2
     # via fastparquet
-cryptography==40.0.1
+cryptography==40.0.2
     # via
     #   dycw-utilities (pyproject.toml)
     #   secretstorage
 cvxpy==1.3.1
     # via dycw-utilities (pyproject.toml)
 cx-oracle==8.3.0
     # via dycw-utilities (pyproject.toml)
@@ -96,15 +96,15 @@
     # via numcodecs
 exceptiongroup==1.1.1
     # via
     #   dycw-utilities (pyproject.toml)
     #   trio-websocket
 execnet==1.9.0
     # via pytest-xdist
-fastapi==0.95.0
+fastapi==0.95.1
     # via dycw-utilities (pyproject.toml)
 fasteners==0.18
     # via zarr
 fastparquet==2023.2.0
     # via dycw-utilities (pyproject.toml)
 filelock==3.11.0
     # via virtualenv
@@ -124,32 +124,32 @@
     #   wsproto
 hatch==1.7.0
     # via dycw-utilities (pyproject.toml)
 hatchling==1.14.0
     # via hatch
 holoviews==1.15.4
     # via dycw-utilities (pyproject.toml)
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via hatch
 hyperlink==21.0.0
     # via hatch
 hypothesis==6.71.0
     # via
     #   dycw-utilities (pyproject.toml)
     #   hypothesis-sqlalchemy
 hypothesis-sqlalchemy==1.1.0
     # via dycw-utilities (pyproject.toml)
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   hyperlink
     #   requests
-    #   rfc3986
     #   trio
 importlib-metadata==6.3.0
     # via keyring
 iniconfig==2.0.0
     # via pytest
 jaraco-classes==3.2.3
     # via keyring
@@ -202,33 +202,33 @@
     #   osqp
     #   pandas
     #   qdldl
     #   scipy
     #   scs
     #   xarray
     #   zarr
-osqp==0.6.2.post8
+osqp==0.6.2.post9
     # via cvxpy
 outcome==1.2.0
     # via trio
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   bokeh
     #   build
     #   coverage-conditional-plugin
     #   fastparquet
     #   hatch
     #   hatchling
     #   holoviews
     #   nox
     #   pytest
     #   pytest-rerunfailures
     #   xarray
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   dycw-utilities (pyproject.toml)
     #   fastparquet
     #   holoviews
     #   xarray
 panel==0.14.4
     # via holoviews
@@ -273,29 +273,29 @@
     # via cffi
 pyct==0.5.0
     # via
     #   colorcet
     #   panel
 pydantic==1.10.7
     # via fastapi
-pygments==2.14.0
+pygments==2.15.0
     # via rich
 pyinstrument==4.4.0
     # via dycw-utilities (pyproject.toml)
-pyodbc==4.0.35
+pyodbc==4.0.39
     # via dycw-utilities (pyproject.toml)
 pyperclip==1.8.2
     # via hatch
 pypi==2.1
     # via dycw-utilities (pyproject.toml)
 pyproject-hooks==1.0.0
     # via build
 pysocks==1.7.1
     # via urllib3
-pytest==7.3.0
+pytest==7.3.1
     # via
     #   dycw-utilities (pyproject.toml)
     #   pytest-check
     #   pytest-cov
     #   pytest-instafail
     #   pytest-randomly
     #   pytest-rerunfailures
@@ -327,17 +327,15 @@
     #   panel
 pyyaml==6.0
     # via bokeh
 qdldl==0.1.7
     # via osqp
 requests==2.28.2
     # via panel
-rfc3986[idna2008]==1.5.0
-    # via httpx
-rich==13.3.3
+rich==13.3.4
     # via hatch
 ruff==0.0.261
     # via dycw-utilities (pyproject.toml)
 scipy==1.10.1
     # via
     #   cvxpy
     #   dycw-utilities (pyproject.toml)
@@ -406,14 +404,16 @@
     # via
     #   bokeh
     #   dycw-utilities (pyproject.toml)
     #   panel
     #   pqdm
     #   pydantic
     #   sqlalchemy
+tzdata==2023.3
+    # via pandas
 urllib3[socks]==1.26.15
     # via
     #   requests
     #   selenium
 userpath==1.8.0
     # via hatch
 virtualenv==20.21.0
@@ -422,15 +422,15 @@
     #   nox
 webencodings==0.5.1
     # via bleach
 wheel==0.40.0
     # via pip-tools
 wsproto==1.2.0
     # via trio-websocket
-xarray==2023.3.0
+xarray==2023.4.0
     # via dycw-utilities (pyproject.toml)
 zarr==2.14.2
     # via dycw-utilities (pyproject.toml)
 zipp==3.15.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `dycw_utilities-0.8.8/.github/workflows/pull-request.yml` & `dycw_utilities-0.9.0/.github/workflows/pull-request.yml`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/.github/workflows/push.yml` & `dycw_utilities-0.9.0/.github/workflows/push.yml`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_airium.py` & `dycw_utilities-0.9.0/tests/test_airium.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_atomicwrites.py` & `dycw_utilities-0.9.0/tests/test_atomicwrites.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_beartype.py` & `dycw_utilities-0.9.0/tests/test_beartype.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_bidict.py` & `dycw_utilities-0.9.0/tests/test_bidict.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_class_name.py` & `dycw_utilities-0.9.0/tests/test_class_name.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_clean_dir.py` & `dycw_utilities-0.9.0/tests/test_clean_dir.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_cryptography.py` & `dycw_utilities-0.9.0/tests/test_cryptography.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_cvxpy.py` & `dycw_utilities-0.9.0/tests/test_cvxpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_datetime.py` & `dycw_utilities-0.9.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_email.py` & `dycw_utilities-0.9.0/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_enum.py` & `dycw_utilities-0.9.0/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_errors.py` & `dycw_utilities-0.9.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_fastapi.py` & `dycw_utilities-0.9.0/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_fastparquet.py` & `dycw_utilities-0.9.0/tests/test_fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_fpdf2.py` & `dycw_utilities-0.9.0/tests/test_fpdf2.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_git.py` & `dycw_utilities-0.9.0/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_hashlib.py` & `dycw_utilities-0.9.0/tests/test_hashlib.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_iterables.py` & `dycw_utilities-0.9.0/tests/test_iterables.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_json.py` & `dycw_utilities-0.9.0/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_modules.py` & `dycw_utilities-0.9.0/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_monitor_memory.py` & `dycw_utilities-0.9.0/tests/test_monitor_memory.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_more_itertools.py` & `dycw_utilities-0.9.0/tests/test_more_itertools.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_os.py` & `dycw_utilities-0.9.0/tests/test_os.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_pathlib.py` & `dycw_utilities-0.9.0/tests/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_pickle.py` & `dycw_utilities-0.9.0/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_pqdm.py` & `dycw_utilities-0.9.0/tests/test_pqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_pypi_server.py` & `dycw_utilities-0.9.0/tests/test_pypi_server.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_pytest.py` & `dycw_utilities-0.9.0/tests/test_pytest.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_pytest_check.py` & `dycw_utilities-0.9.0/tests/test_pytest_check.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_re.py` & `dycw_utilities-0.9.0/tests/test_re.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_scipy.py` & `dycw_utilities-0.9.0/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_subprocess.py` & `dycw_utilities-0.9.0/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_tempfile.py` & `dycw_utilities-0.9.0/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_text.py` & `dycw_utilities-0.9.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_timer.py` & `dycw_utilities-0.9.0/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_tqdm.py` & `dycw_utilities-0.9.0/tests/test_tqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_typed_settings.py` & `dycw_utilities-0.9.0/tests/test_typed_settings.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_types.py` & `dycw_utilities-0.9.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_warnings.py` & `dycw_utilities-0.9.0/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/test_zipfile.py` & `dycw_utilities-0.9.0/tests/test_zipfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/attrs/test_attrs.py` & `dycw_utilities-0.9.0/tests/attrs/test_attrs.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/attrs/test_xarray.py` & `dycw_utilities-0.9.0/tests/attrs/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/click/test_click.py` & `dycw_utilities-0.9.0/tests/click/test_click.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/click/test_luigi.py` & `dycw_utilities-0.9.0/tests/click/test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/click/test_sqlalchemy.py` & `dycw_utilities-0.9.0/tests/click/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/holoviews/test_holoviews.py` & `dycw_utilities-0.9.0/tests/holoviews/test_holoviews.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/holoviews/test_xarray.py` & `dycw_utilities-0.9.0/tests/holoviews/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/hypothesis/test_hypothesis.py` & `dycw_utilities-0.9.0/tests/hypothesis/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/hypothesis/test_luigi.py` & `dycw_utilities-0.9.0/tests/hypothesis/test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/hypothesis/test_numpy.py` & `dycw_utilities-0.9.0/tests/hypothesis/test_numpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/hypothesis/test_pandas.py` & `dycw_utilities-0.9.0/tests/hypothesis/test_pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/hypothesis/test_semver.py` & `dycw_utilities-0.9.0/tests/hypothesis/test_semver.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/hypothesis/test_sqlalchemy.py` & `dycw_utilities-0.9.0/tests/hypothesis/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/hypothesis/test_xarray.py` & `dycw_utilities-0.9.0/tests/hypothesis/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/loguru/script_to_test_luigi.py` & `dycw_utilities-0.9.0/tests/loguru/script_to_test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/loguru/test_loguru.py` & `dycw_utilities-0.9.0/tests/loguru/test_loguru.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/luigi/test_attrs.py` & `dycw_utilities-0.9.0/tests/luigi/test_attrs.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/luigi/test_luigi.py` & `dycw_utilities-0.9.0/tests/luigi/test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/luigi/test_server.py` & `dycw_utilities-0.9.0/tests/luigi/test_server.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/luigi/test_sqlalchemy.py` & `dycw_utilities-0.9.0/tests/luigi/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/math/test_math.py` & `dycw_utilities-0.9.0/tests/math/test_math.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/math/test_typing.py` & `dycw_utilities-0.9.0/tests/math/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/numpy/test_numpy.py` & `dycw_utilities-0.9.0/tests/numpy/test_numpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/numpy/test_typing.py` & `dycw_utilities-0.9.0/tests/numpy/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/pandas/test_pandas.py` & `dycw_utilities-0.9.0/tests/pandas/test_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,26 +127,26 @@
     @beartype
     def test_series_pass(self) -> None:
         series = Series(index=RangeIndex(0), dtype=float)
         check_range_index(series)
 
     @beartype
     def test_series_fail(self) -> None:
-        series = Series(dtype=float)
+        series = Series(index=Index([], dtype=int), dtype=float)
         with raises(SeriesRangeIndexError):
             check_range_index(series)
 
     @beartype
     def test_dataframe_pass(self) -> None:
         df = DataFrame(index=RangeIndex(0))
         check_range_index(df)
 
     @beartype
     def test_dataframe_fail(self) -> None:
-        df = DataFrame()
+        df = DataFrame(index=Index([], dtype=int))
         with raises(DataFrameRangeIndexError):
             check_range_index(df)
 
 
 class TestDTypes:
     @mark.parametrize("dtype", [param(Int64), param(boolean), param(string)])
     @beartype
```

### Comparing `dycw_utilities-0.8.8/tests/pandas/test_typing.py` & `dycw_utilities-0.9.0/tests/pandas/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/sqlalchemy/test_fastparquet.py` & `dycw_utilities-0.9.0/tests/sqlalchemy/test_fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/sqlalchemy/test_pandas.py` & `dycw_utilities-0.9.0/tests/sqlalchemy/test_pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/sqlalchemy/test_sqlalchemy.py` & `dycw_utilities-0.9.0/tests/sqlalchemy/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/xarray/test_typing.py` & `dycw_utilities-0.9.0/tests/xarray/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/zarr/test_xarray.py` & `dycw_utilities-0.9.0/tests/zarr/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/tests/zarr/test_zarr.py` & `dycw_utilities-0.9.0/tests/zarr/test_zarr.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/atomicwrites.py` & `dycw_utilities-0.9.0/utilities/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/bidict.py` & `dycw_utilities-0.9.0/utilities/bidict.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/cryptography.py` & `dycw_utilities-0.9.0/utilities/cryptography.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/cvxpy.py` & `dycw_utilities-0.9.0/utilities/cvxpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/datetime.py` & `dycw_utilities-0.9.0/utilities/datetime.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/email.py` & `dycw_utilities-0.9.0/utilities/email.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/enum.py` & `dycw_utilities-0.9.0/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/errors.py` & `dycw_utilities-0.9.0/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/fastapi.py` & `dycw_utilities-0.9.0/utilities/fastapi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/fastparquet.py` & `dycw_utilities-0.9.0/utilities/fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/fpdf2.py` & `dycw_utilities-0.9.0/utilities/fpdf2.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/git.py` & `dycw_utilities-0.9.0/utilities/git.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/hatch.py` & `dycw_utilities-0.9.0/utilities/hatch.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/iterables.py` & `dycw_utilities-0.9.0/utilities/iterables.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/json.py` & `dycw_utilities-0.9.0/utilities/json.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/logging.py` & `dycw_utilities-0.9.0/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/loguru.py` & `dycw_utilities-0.9.0/utilities/loguru.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/memory_profiler.py` & `dycw_utilities-0.9.0/utilities/memory_profiler.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/modules.py` & `dycw_utilities-0.9.0/utilities/modules.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/more_itertools.py` & `dycw_utilities-0.9.0/utilities/more_itertools.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/os.py` & `dycw_utilities-0.9.0/utilities/os.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/pickle.py` & `dycw_utilities-0.9.0/utilities/pickle.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/pqdm.py` & `dycw_utilities-0.9.0/utilities/pqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/pyinstrument.py` & `dycw_utilities-0.9.0/utilities/pyinstrument.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/pytest.py` & `dycw_utilities-0.9.0/utilities/pytest.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/re.py` & `dycw_utilities-0.9.0/utilities/re.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/scipy.py` & `dycw_utilities-0.9.0/utilities/scipy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/sentinel.py` & `dycw_utilities-0.9.0/utilities/sentinel.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/subprocess.py` & `dycw_utilities-0.9.0/utilities/subprocess.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/tempfile.py` & `dycw_utilities-0.9.0/utilities/tempfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/text.py` & `dycw_utilities-0.9.0/utilities/text.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/timer.py` & `dycw_utilities-0.9.0/utilities/timer.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/tqdm.py` & `dycw_utilities-0.9.0/utilities/tqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/typed_settings.py` & `dycw_utilities-0.9.0/utilities/typed_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 @beartype
 def get_repo_root_config(
     *, cwd: PathLike = Path.cwd(), filename: str = "config.toml"
 ) -> Optional[Path]:
     """Get the config under the repo root, if it exists."""
     try:
         root = get_repo_root(cwd=cwd)
-    except InvalidRepoError:
+    except (FileNotFoundError, InvalidRepoError):
         return None
     if (path := root.joinpath(filename)).exists():
         return path
     return None
 
 
 _CONFIG_FILES = [p for p in [get_repo_root_config()] if p is not None]
```

### Comparing `dycw_utilities-0.8.8/utilities/types.py` & `dycw_utilities-0.9.0/utilities/types.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/warnings.py` & `dycw_utilities-0.9.0/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/zipfile.py` & `dycw_utilities-0.9.0/utilities/zipfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/attrs/__init__.py` & `dycw_utilities-0.9.0/utilities/attrs/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/clean_dir/__init__.py` & `dycw_utilities-0.9.0/utilities/clean_dir/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/clean_dir/classes.py` & `dycw_utilities-0.9.0/utilities/clean_dir/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/click/__init__.py` & `dycw_utilities-0.9.0/utilities/click/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/click/luigi.py` & `dycw_utilities-0.9.0/utilities/click/luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/click/sqlalchemy.py` & `dycw_utilities-0.9.0/utilities/click/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/holoviews/__init__.py` & `dycw_utilities-0.9.0/utilities/holoviews/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/holoviews/xarray.py` & `dycw_utilities-0.9.0/utilities/holoviews/xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/hypothesis/__init__.py` & `dycw_utilities-0.9.0/utilities/hypothesis/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/hypothesis/numpy.py` & `dycw_utilities-0.9.0/utilities/hypothesis/numpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/hypothesis/pandas.py` & `dycw_utilities-0.9.0/utilities/hypothesis/pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/hypothesis/semver.py` & `dycw_utilities-0.9.0/utilities/hypothesis/semver.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/hypothesis/sqlalchemy.py` & `dycw_utilities-0.9.0/utilities/hypothesis/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/hypothesis/xarray.py` & `dycw_utilities-0.9.0/utilities/hypothesis/xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/luigi/__init__.py` & `dycw_utilities-0.9.0/utilities/luigi/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/luigi/attrs.py` & `dycw_utilities-0.9.0/utilities/luigi/attrs.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/luigi/semver.py` & `dycw_utilities-0.9.0/utilities/luigi/semver.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/luigi/sqlalchemy.py` & `dycw_utilities-0.9.0/utilities/luigi/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/luigi/server/__init__.py` & `dycw_utilities-0.9.0/utilities/luigi/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/luigi/server/classes.py` & `dycw_utilities-0.9.0/utilities/luigi/server/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/math/__init__.py` & `dycw_utilities-0.9.0/utilities/math/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/math/typing.py` & `dycw_utilities-0.9.0/utilities/math/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/monitor_memory/__init__.py` & `dycw_utilities-0.9.0/utilities/monitor_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/monitor_memory/classes.py` & `dycw_utilities-0.9.0/utilities/monitor_memory/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/numpy/__init__.py` & `dycw_utilities-0.9.0/utilities/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/numpy/typing.py` & `dycw_utilities-0.9.0/utilities/numpy/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/pandas/__init__.py` & `dycw_utilities-0.9.0/utilities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/pandas/typing.py` & `dycw_utilities-0.9.0/utilities/pandas/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/pypi_server/__init__.py` & `dycw_utilities-0.9.0/utilities/pypi_server/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/pypi_server/classes.py` & `dycw_utilities-0.9.0/utilities/pypi_server/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/sqlalchemy/__init__.py` & `dycw_utilities-0.9.0/utilities/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/sqlalchemy/fastparquet.py` & `dycw_utilities-0.9.0/utilities/sqlalchemy/fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/sqlalchemy/pandas.py` & `dycw_utilities-0.9.0/utilities/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/xarray/typing.py` & `dycw_utilities-0.9.0/utilities/xarray/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/zarr/__init__.py` & `dycw_utilities-0.9.0/utilities/zarr/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/utilities/zarr/xarray.py` & `dycw_utilities-0.9.0/utilities/zarr/xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/.gitignore` & `dycw_utilities-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/README.md` & `dycw_utilities-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.8/pyproject.toml` & `dycw_utilities-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -50,25 +50,25 @@
 #### project ##################################################################
 [project]
 name = "dycw-utilities"
 dynamic = ["version"]
 readme = "README.md"
 requires-python = ">= 3.9"
 authors = [{ name = "Derek Wan", email = "d.wan@icloud.com" }]
-dependencies = ["beartype >= 0.13.0", "typing-extensions >= 4.5.0"]
+dependencies = ["beartype >= 0.13.1", "typing-extensions >= 4.5.0"]
 
 [project.optional-dependencies]
 airium = ["airium >= 0.2.5"]
 atomicwrites = ["atomicwrites >= 1.4.1"]
 attrs = ["attrs >= 22.2.0"]
 bidict = ["bidict >= 0.22.1"]
 click = ["click >= 8.1.3"]
-cryptography = ["cryptography >= 40.0.1"]
+cryptography = ["cryptography >= 40.0.2"]
 cvxpy = ["cvxpy >= 1.3.1"]
-fastapi = ["fastapi >= 0.95.0"]
+fastapi = ["fastapi >= 0.95.1"]
 fastparquet = [
   "atomicwrites >= 1.4.1",
   "fastparquet >= 2023.2.0",
 ]
 fpdf2 = [
   "atomicwrites >= 1.4.1",
   "fpdf2 >= 2.7.3",
@@ -89,30 +89,30 @@
 numpy = [
   "bottleneck >= 1.3.7",
   "numpy >= 1.23.5",
 ]
 pandas = [
   "bottleneck >= 1.3.7",
   "numpy >= 1.23.5",
-  "pandas >= 1.5.3",
+  "pandas >= 2.0.0",
 ]
 pqdm = ["pqdm >= 0.2.0"]
 psutil = ["psutil >= 5.9.4"]
 pyinstrument = [
   "atomicwrites >= 1.4.1",
   "pyinstrument >= 4.4.0",
 ]
 pypi = [
   "loguru >= 0.7.0",
   "pypiserver[passlib] >= 1.5.1",
   "typed-settings[click] >= 23.0.0",
 ]
 pytest = [
   "atomicwrites >= 1.4.1",
-  "pytest >= 7.3.0",
+  "pytest >= 7.3.1",
 ]
 pytest-check = ["pytest-check >= 2.1.4"]
 scipy = ["scipy >= 1.10.1, < 1.11"]
 scripts = [
   "loguru >= 0.7.0",
   "typed-settings[click] >= 23.0.0",
 ]
@@ -124,54 +124,54 @@
   "timeout-decorator >= 0.5.0",
 ]
 tqdm = ["tqdm >= 4.65.0"]
 typed-settings = ["typed-settings[click] >= 23.0.0"]
 xarray = [
   "bottleneck >= 1.3.7",
   "numpy >= 1.23.5",
-  "xarray >= 2023.2.0",
+  "xarray >= 2023.4.0",
 ]
 zarr = [
   "atomicwrites >= 1.4.1",
   "zarr >= 2.14.2",
 ]
 # groups
 core = [
   "airium >= 0.2.5",
   "atomicwrites >= 1.4.1",
   "attrs >= 22.2.0",
   "bidict >= 0.22.1",
   "bottleneck >= 1.3.7",
   "click >= 8.1.3",
-  "cryptography >= 40.0.1",
+  "cryptography >= 40.0.2",
   "cvxpy >= 1.3.1",
   "fastparquet >= 2023.2.0",
   "fpdf2 >= 2.7.3",
   "holoviews >= 1.15.4",
   "loguru >= 0.7.0",
   "luigi >= 3.2.1",
   "more-itertools >= 9.1.0",
   "numpy >= 1.23.5",
-  "pandas >= 1.5.3",
+  "pandas >= 2.0.0",
   "pqdm >= 0.2.0",
   "selenium >= 4.8.3",
   "semver >= 3.0.0",
   "scipy >= 1.10.1, < 1.11",
   "sqlalchemy >= 2.0.9",
   "timeout-decorator >= 0.5.0, < 0.6",
   "tqdm >= 4.65.0",
   "typed-settings[click] >= 23.0.0",
-  "xarray >= 2023.2.0",
+  "xarray >= 2023.4.0",
   "zarr >= 2.14.2",
 ]
 test = [
   "atomicwrites >= 1.4.1",
   "exceptiongroup >= 1.1.1",
   "hypothesis >= 6.71.0",
-  "pytest >= 7.3.0",
+  "pytest >= 7.3.1",
   "pytest-check >= 2.1.4",
   "pytest-cov >= 4.0.0",
   "pytest-instafail >= 0.5.0",
   "pytest-randomly >= 3.12.0",
   "pytest-rerunfailures >= 11.1.2",
   "pytest-xdist >= 3.2.1",
 ]
```

### Comparing `dycw_utilities-0.8.8/PKG-INFO` & `dycw_utilities-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dycw-utilities
-Version: 0.8.8
+Version: 0.9.0
 Author-email: Derek Wan <d.wan@icloud.com>
 Requires-Python: >=3.9
-Requires-Dist: beartype>=0.13.0
+Requires-Dist: beartype>=0.13.1
 Requires-Dist: typing-extensions>=4.5.0
 Provides-Extra: airium
 Requires-Dist: airium>=0.2.5; extra == 'airium'
 Provides-Extra: atomicwrites
 Requires-Dist: atomicwrites>=1.4.1; extra == 'atomicwrites'
 Provides-Extra: attrs
 Requires-Dist: attrs>=22.2.0; extra == 'attrs'
@@ -18,36 +18,36 @@
 Provides-Extra: core
 Requires-Dist: airium>=0.2.5; extra == 'core'
 Requires-Dist: atomicwrites>=1.4.1; extra == 'core'
 Requires-Dist: attrs>=22.2.0; extra == 'core'
 Requires-Dist: bidict>=0.22.1; extra == 'core'
 Requires-Dist: bottleneck>=1.3.7; extra == 'core'
 Requires-Dist: click>=8.1.3; extra == 'core'
-Requires-Dist: cryptography>=40.0.1; extra == 'core'
+Requires-Dist: cryptography>=40.0.2; extra == 'core'
 Requires-Dist: cvxpy>=1.3.1; extra == 'core'
 Requires-Dist: fastparquet>=2023.2.0; extra == 'core'
 Requires-Dist: fpdf2>=2.7.3; extra == 'core'
 Requires-Dist: holoviews>=1.15.4; extra == 'core'
 Requires-Dist: loguru>=0.7.0; extra == 'core'
 Requires-Dist: luigi>=3.2.1; extra == 'core'
 Requires-Dist: more-itertools>=9.1.0; extra == 'core'
 Requires-Dist: numpy>=1.23.5; extra == 'core'
-Requires-Dist: pandas>=1.5.3; extra == 'core'
+Requires-Dist: pandas>=2.0.0; extra == 'core'
 Requires-Dist: pqdm>=0.2.0; extra == 'core'
 Requires-Dist: scipy<1.11,>=1.10.1; extra == 'core'
 Requires-Dist: selenium>=4.8.3; extra == 'core'
 Requires-Dist: semver>=3.0.0; extra == 'core'
 Requires-Dist: sqlalchemy>=2.0.9; extra == 'core'
 Requires-Dist: timeout-decorator<0.6,>=0.5.0; extra == 'core'
 Requires-Dist: tqdm>=4.65.0; extra == 'core'
 Requires-Dist: typed-settings[click]>=23.0.0; extra == 'core'
-Requires-Dist: xarray>=2023.2.0; extra == 'core'
+Requires-Dist: xarray>=2023.4.0; extra == 'core'
 Requires-Dist: zarr>=2.14.2; extra == 'core'
 Provides-Extra: cryptography
-Requires-Dist: cryptography>=40.0.1; extra == 'cryptography'
+Requires-Dist: cryptography>=40.0.2; extra == 'cryptography'
 Provides-Extra: cvxpy
 Requires-Dist: cvxpy>=1.3.1; extra == 'cvxpy'
 Provides-Extra: dev
 Requires-Dist: airium; extra == 'dev'
 Requires-Dist: atomicwrites; extra == 'dev'
 Requires-Dist: attrs; extra == 'dev'
 Requires-Dist: bidict; extra == 'dev'
@@ -96,15 +96,15 @@
 Requires-Dist: sqlalchemy; extra == 'dev'
 Requires-Dist: timeout-decorator; extra == 'dev'
 Requires-Dist: tqdm; extra == 'dev'
 Requires-Dist: typed-settings[click]; extra == 'dev'
 Requires-Dist: xarray; extra == 'dev'
 Requires-Dist: zarr; extra == 'dev'
 Provides-Extra: fastapi
-Requires-Dist: fastapi>=0.95.0; extra == 'fastapi'
+Requires-Dist: fastapi>=0.95.1; extra == 'fastapi'
 Provides-Extra: fastparquet
 Requires-Dist: atomicwrites>=1.4.1; extra == 'fastparquet'
 Requires-Dist: fastparquet>=2023.2.0; extra == 'fastparquet'
 Provides-Extra: fpdf2
 Requires-Dist: atomicwrites>=1.4.1; extra == 'fpdf2'
 Requires-Dist: fpdf2>=2.7.3; extra == 'fpdf2'
 Requires-Dist: holoviews>=1.15.4; extra == 'fpdf2'
@@ -127,29 +127,29 @@
 Requires-Dist: more-itertools>=9.1.0; extra == 'more-itertools'
 Provides-Extra: numpy
 Requires-Dist: bottleneck>=1.3.7; extra == 'numpy'
 Requires-Dist: numpy>=1.23.5; extra == 'numpy'
 Provides-Extra: pandas
 Requires-Dist: bottleneck>=1.3.7; extra == 'pandas'
 Requires-Dist: numpy>=1.23.5; extra == 'pandas'
-Requires-Dist: pandas>=1.5.3; extra == 'pandas'
+Requires-Dist: pandas>=2.0.0; extra == 'pandas'
 Provides-Extra: pqdm
 Requires-Dist: pqdm>=0.2.0; extra == 'pqdm'
 Provides-Extra: psutil
 Requires-Dist: psutil>=5.9.4; extra == 'psutil'
 Provides-Extra: pyinstrument
 Requires-Dist: atomicwrites>=1.4.1; extra == 'pyinstrument'
 Requires-Dist: pyinstrument>=4.4.0; extra == 'pyinstrument'
 Provides-Extra: pypi
 Requires-Dist: loguru>=0.7.0; extra == 'pypi'
 Requires-Dist: pypiserver[passlib]>=1.5.1; extra == 'pypi'
 Requires-Dist: typed-settings[click]>=23.0.0; extra == 'pypi'
 Provides-Extra: pytest
 Requires-Dist: atomicwrites>=1.4.1; extra == 'pytest'
-Requires-Dist: pytest>=7.3.0; extra == 'pytest'
+Requires-Dist: pytest>=7.3.1; extra == 'pytest'
 Provides-Extra: pytest-check
 Requires-Dist: pytest-check>=2.1.4; extra == 'pytest-check'
 Provides-Extra: scipy
 Requires-Dist: scipy<1.11,>=1.10.1; extra == 'scipy'
 Provides-Extra: scripts
 Requires-Dist: loguru>=0.7.0; extra == 'scripts'
 Requires-Dist: typed-settings[click]>=23.0.0; extra == 'scripts'
@@ -166,23 +166,23 @@
 Requires-Dist: hypothesis>=6.71.0; extra == 'test'
 Requires-Dist: pytest-check>=2.1.4; extra == 'test'
 Requires-Dist: pytest-cov>=4.0.0; extra == 'test'
 Requires-Dist: pytest-instafail>=0.5.0; extra == 'test'
 Requires-Dist: pytest-randomly>=3.12.0; extra == 'test'
 Requires-Dist: pytest-rerunfailures>=11.1.2; extra == 'test'
 Requires-Dist: pytest-xdist>=3.2.1; extra == 'test'
-Requires-Dist: pytest>=7.3.0; extra == 'test'
+Requires-Dist: pytest>=7.3.1; extra == 'test'
 Provides-Extra: tqdm
 Requires-Dist: tqdm>=4.65.0; extra == 'tqdm'
 Provides-Extra: typed-settings
 Requires-Dist: typed-settings[click]>=23.0.0; extra == 'typed-settings'
 Provides-Extra: xarray
 Requires-Dist: bottleneck>=1.3.7; extra == 'xarray'
 Requires-Dist: numpy>=1.23.5; extra == 'xarray'
-Requires-Dist: xarray>=2023.2.0; extra == 'xarray'
+Requires-Dist: xarray>=2023.4.0; extra == 'xarray'
 Provides-Extra: zarr
 Requires-Dist: atomicwrites>=1.4.1; extra == 'zarr'
 Requires-Dist: zarr>=2.14.2; extra == 'zarr'
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/dycw-utilities.svg)](https://badge.fury.io/py/dycw-utilities)
```

