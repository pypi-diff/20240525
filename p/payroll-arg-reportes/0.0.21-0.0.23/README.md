# Comparing `tmp/payroll_arg_reportes-0.0.21.tar.gz` & `tmp/payroll_arg_reportes-0.0.23.tar.gz`

## Comparing `payroll_arg_reportes-0.0.21.tar` & `payroll_arg_reportes-0.0.23.tar`

### file list

```diff
@@ -1,45 +1,64 @@
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/.github/workflows/tests.yml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/docs/f931.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/docs/libro-de-sueldos.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/docs/pypi-publish.md
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/docs/recibo-de-sueldos.md
--rw-r--r--   0        0        0   285657 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/docs/images/libro-sueldo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/__init__.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/config.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/logs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/base_reports/__init__.py
--rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/base_reports/recibo_base_1.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/__init__.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/descarga_excel.py
--rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/recibo_sueldo.py
--rw-r--r--   0        0        0     7741 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/f931/reporter.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/f931/tools.py
--rwxr-xr-x   0        0        0    17144 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/f931/samples/Formato_SICOSS_v42.pdf
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/f931/samples/f931-info.json
--rw-r--r--   0        0        0     9675 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/libro_sueldo/__init__.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/libro_sueldo/data.py
--rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/libro_sueldo/samples/samples-recibo-info.json
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/reporters/samples/samples-recibo-info.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/tables/base_tables.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/test_cases/f931-info.json
--rw-r--r--   0        0        0   154914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/test_cases/liquidacion_completa.json
--rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/test_cases/liquidacion_corta.json
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/test_cases/test_f931.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/test_cases/test_libro_sueldo.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/test_cases/test_recibo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/tools/__init__.py
--rw-r--r--   0        0        0    14126 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/tools/base.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/py_arg_reports/tools/recibos_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/tests/__init__.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/tests/test_download_recibo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/tests/f931/__init__.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/tests/f931/test_generacion_f931.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/tests/libro_sueldo/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/tests/libro_sueldo/test_base_pdf.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/LICENSE
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/README.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/pyproject.toml
--rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/docs/acreditaciones-santander.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/docs/f931.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/docs/libro-de-sueldos.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/docs/pypi-publish.md
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/docs/recibo-de-sueldos.md
+-rw-r--r--   0        0        0   285657 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/docs/images/libro-sueldo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/config.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/logs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/base_reports/__init__.py
+-rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/base_reports/recibo_base_1.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/__init__.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/descarga_excel.py
+-rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/recibo_sueldo.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/README.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/__init__.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/base.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/data/bancos.json
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/data/bancos.wikipedia
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/data/sample.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/nacion/docs/README.md
+-rw-r--r--   0        0        0   123581 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/nacion/docs/detalle-registro.png
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/santander/README.md
+-rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/santander/__init__.py
+-rw-r--r--   0        0        0   132456 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/santander/docs/Guia Pago Simple.xlsx
+-rw-r--r--   0        0        0   183476 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/santander/docs/Guía txt - Pago de Haberes y Honorarios.pdf
+-rw-r--r--   0        0        0   429174 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/santander/docs/Guía txt - Pago de Proveedores, Personalizados y Seguro.pdf
+-rw-r--r--   0        0        0    94589 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/acreditaciones/santander/docs/screenshot-santander.png
+-rw-r--r--   0        0        0     7741 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/f931/reporter.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/f931/tools.py
+-rwxr-xr-x   0        0        0    17144 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/f931/samples/Formato_SICOSS_v42.pdf
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/f931/samples/f931-info.json
+-rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/libro_sueldo/__init__.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/libro_sueldo/data.py
+-rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/libro_sueldo/samples/samples-recibo-info.json
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/reporters/samples/samples-recibo-info.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/tables/base_tables.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/test_cases/f931-info.json
+-rw-r--r--   0        0        0   154914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/test_cases/liquidacion_completa.json
+-rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/test_cases/liquidacion_corta.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/test_cases/test_f931.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/test_cases/test_libro_sueldo.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/test_cases/test_recibo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/tools/__init__.py
+-rw-r--r--   0        0        0    14126 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/tools/pdf.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/tools/recibos_utils.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/py_arg_reports/tools/txt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/tests/__init__.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/tests/test_download_recibo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/tests/acreditaciones/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/tests/acreditaciones/santander/__init__.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/tests/acreditaciones/santander/test_base_acreditacion_santander.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/tests/f931/__init__.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/tests/f931/test_generacion_f931.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/tests/libro_sueldo/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/tests/libro_sueldo/test_base_pdf.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/LICENSE
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/README.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/pyproject.toml
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.23/PKG-INFO
```

### Comparing `payroll_arg_reportes-0.0.21/.github/workflows/python-publish.yml` & `payroll_arg_reportes-0.0.23/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/.github/workflows/tests.yml` & `payroll_arg_reportes-0.0.23/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/docs/f931.md` & `payroll_arg_reportes-0.0.23/docs/f931.md`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/docs/libro-de-sueldos.md` & `payroll_arg_reportes-0.0.23/docs/libro-de-sueldos.md`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/docs/pypi-publish.md` & `payroll_arg_reportes-0.0.23/docs/pypi-publish.md`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/docs/recibo-de-sueldos.md` & `payroll_arg_reportes-0.0.23/docs/recibo-de-sueldos.md`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/docs/images/libro-sueldo.png` & `payroll_arg_reportes-0.0.23/docs/images/libro-sueldo.png`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/base_reports/recibo_base_1.py` & `payroll_arg_reportes-0.0.23/py_arg_reports/base_reports/recibo_base_1.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/reporters/descarga_excel.py` & `payroll_arg_reportes-0.0.23/py_arg_reports/reporters/descarga_excel.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/reporters/recibo_sueldo.py` & `payroll_arg_reportes-0.0.23/py_arg_reports/reporters/recibo_sueldo.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/reporters/f931/reporter.py` & `payroll_arg_reportes-0.0.23/py_arg_reports/reporters/f931/reporter.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/reporters/f931/tools.py` & `payroll_arg_reportes-0.0.23/py_arg_reports/reporters/f931/tools.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/reporters/f931/samples/Formato_SICOSS_v42.pdf` & `payroll_arg_reportes-0.0.23/py_arg_reports/reporters/f931/samples/Formato_SICOSS_v42.pdf`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/reporters/f931/samples/f931-info.json` & `payroll_arg_reportes-0.0.23/py_arg_reports/reporters/f931/samples/f931-info.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/reporters/libro_sueldo/__init__.py` & `payroll_arg_reportes-0.0.23/py_arg_reports/reporters/libro_sueldo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from py_arg_reports.logs import get_logger
 from py_arg_reports.reporters.libro_sueldo.data import translate_data
-from py_arg_reports.tools.base import CanvasPDF, CanvaPDFBlock, Format, Rect
+from py_arg_reports.tools.pdf import CanvasPDF, CanvaPDFBlock, Format, Rect
 from py_arg_reports.tools.recibos_utils import float_to_format_currency
 from reportlab.lib.units import cm
 
 
 log = get_logger(__name__)
 F14 = Format(font_size=14)
 F10 = Format(font_size=10)
```

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/reporters/libro_sueldo/data.py` & `payroll_arg_reportes-0.0.23/py_arg_reports/reporters/libro_sueldo/data.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/reporters/libro_sueldo/samples/samples-recibo-info.json` & `payroll_arg_reportes-0.0.23/py_arg_reports/reporters/libro_sueldo/samples/samples-recibo-info.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/reporters/samples/samples-recibo-info.json` & `payroll_arg_reportes-0.0.23/py_arg_reports/reporters/samples/samples-recibo-info.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/test_cases/f931-info.json` & `payroll_arg_reportes-0.0.23/py_arg_reports/test_cases/f931-info.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/test_cases/liquidacion_completa.json` & `payroll_arg_reportes-0.0.23/py_arg_reports/test_cases/liquidacion_completa.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/test_cases/liquidacion_corta.json` & `payroll_arg_reportes-0.0.23/py_arg_reports/test_cases/liquidacion_corta.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/tools/base.py` & `payroll_arg_reportes-0.0.23/py_arg_reports/tools/pdf.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/py_arg_reports/tools/recibos_utils.py` & `payroll_arg_reportes-0.0.23/py_arg_reports/tools/recibos_utils.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/tests/test_download_recibo.py` & `payroll_arg_reportes-0.0.23/tests/test_download_recibo.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/tests/f931/test_generacion_f931.py` & `payroll_arg_reportes-0.0.23/tests/f931/test_generacion_f931.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/tests/libro_sueldo/test_base_pdf.py` & `payroll_arg_reportes-0.0.23/tests/libro_sueldo/test_base_pdf.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/LICENSE` & `payroll_arg_reportes-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.21/README.md` & `payroll_arg_reportes-0.0.23/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 - UTHGRA
 - Etc.
 
 
 ### Reportes Bancarios
 
 - Banco Galicia
-- Banco Santander
+- [Banco Santander](https://github.com/Artimezoft/payroll_arg_reportes/blob/develop/docs/acreditaciones-santander.md)
 - Banco Nación
 - Etc.
 
 
 ### Reportes de Liquidación
 
 - Resumen de Liquidación
```

### Comparing `payroll_arg_reportes-0.0.21/pyproject.toml` & `payroll_arg_reportes-0.0.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "payroll_arg_reportes"
-version = "0.0.21"
+version = "0.0.23"
 dependencies = [
   "numero-a-letras>=0.0.4",
   "reportlab==4.0.8",
   "XlsxWriter==3.2.0",
 ]
 requires-python = ">=3.10"
 authors = [
```

### Comparing `payroll_arg_reportes-0.0.21/PKG-INFO` & `payroll_arg_reportes-0.0.23/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: payroll_arg_reportes
-Version: 0.0.21
+Version: 0.0.23
 Summary: Reportes para Payroll en Argentina
 Project-URL: Homepage, https://github.com/Artimezoft/payroll_arg_reportes
 Project-URL: Issues, https://github.com/Artimezoft/payroll_arg_reportes/issues
 Author-email: Eugenio <coding_with@eugeniovazquez.com.ar>, Andres <andres@data99.com.ar>
 Maintainer-email: Eugenio <coding_with@eugeniovazquez.com.ar>, Andres <andres@data99.com.ar>
 License: MIT License
         
@@ -71,15 +71,15 @@
 - UTHGRA
 - Etc.
 
 
 ### Reportes Bancarios
 
 - Banco Galicia
-- Banco Santander
+- [Banco Santander](https://github.com/Artimezoft/payroll_arg_reportes/blob/develop/docs/acreditaciones-santander.md)
 - Banco Nación
 - Etc.
 
 
 ### Reportes de Liquidación
 
 - Resumen de Liquidación
```

