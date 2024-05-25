# Comparing `tmp/odoo_addon_upgrade_analysis-17.0.1.0.0.6-py3-none-any.whl.zip` & `tmp/odoo_addon_upgrade_analysis-17.0.1.0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,56 +1,56 @@
-Zip file size: 65856 bytes, number of entries: 54
--rw-r--r--  2.0 unx     4578 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/README.rst
--rw-r--r--  2.0 unx      140 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/__init__.py
--rw-r--r--  2.0 unx     1077 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/__manifest__.py
--rw-r--r--  2.0 unx      456 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/blacklist.py
--rw-r--r--  2.0 unx    19987 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/compare.py
--rw-r--r--  2.0 unx     8286 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/upgrade_log.py
--rw-r--r--  2.0 unx    22496 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/i18n/es_AR.po
--rw-r--r--  2.0 unx    20161 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/i18n/fr.po
--rw-r--r--  2.0 unx    18533 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
--rw-r--r--  2.0 unx      163 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/__init__.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/ir_module_module.py
--rw-r--r--  2.0 unx    22565 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/upgrade_analysis.py
--rw-r--r--  2.0 unx      536 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/upgrade_attribute.py
--rw-r--r--  2.0 unx     3098 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py
--rw-r--r--  2.0 unx     5998 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/upgrade_record.py
--rw-r--r--  2.0 unx       65 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/__init__.py
--rw-r--r--  2.0 unx     1835 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py
--rw-r--r--  2.0 unx       66 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py
--rw-r--r--  2.0 unx      270 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
--rw-r--r--  2.0 unx      371 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
--rw-r--r--  2.0 unx      259 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
--rw-r--r--  2.0 unx       84 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
--rw-r--r--  2.0 unx      729 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
--rw-r--r--  2.0 unx       19 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py
--rw-r--r--  2.0 unx       23 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py
--rw-r--r--  2.0 unx     1589 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py
--rw-r--r--  2.0 unx       23 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py
--rw-r--r--  2.0 unx     1112 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py
--rw-r--r--  2.0 unx       22 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
--rw-r--r--  2.0 unx      397 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
--rw-r--r--  2.0 unx      336 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.md
--rw-r--r--  2.0 unx      677 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/readme/DESCRIPTION.md
--rw-r--r--  2.0 unx      267 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/readme/ROADMAP.md
--rw-r--r--  2.0 unx       69 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/readme/USAGE.md
--rw-r--r--  2.0 unx      696 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/security/ir.model.access.csv
--rw-r--r--  2.0 unx     9455 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/static/description/icon.png
--rw-r--r--  2.0 unx    15067 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/static/description/index.html
--rw-r--r--  2.0 unx      752 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako
--rw-r--r--  2.0 unx       26 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/tests/__init__.py
--rw-r--r--  2.0 unx     1787 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/tests/test_module.py
--rw-r--r--  2.0 unx      200 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/views/menu.xml
--rw-r--r--  2.0 unx     2250 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml
--rw-r--r--  2.0 unx     2826 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml
--rw-r--r--  2.0 unx     2814 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml
--rw-r--r--  2.0 unx       82 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/wizards/__init__.py
--rw-r--r--  2.0 unx     4527 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py
--rw-r--r--  2.0 unx     4066 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py
--rw-r--r--  2.0 unx     1919 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
--rw-r--r--  2.0 unx     3454 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
--rw-r--r--  2.0 unx     5276 b- defN 24-May-23 11:02 odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       83 b- defN 24-May-23 11:02 odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-May-23 11:02 odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6021 b- defN 24-May-23 11:02 odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/RECORD
-54 files, 198644 bytes uncompressed, 55664 bytes compressed:  72.0%
+Zip file size: 65684 bytes, number of entries: 54
+-rw-r--r--  2.0 unx     4578 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/README.rst
+-rw-r--r--  2.0 unx      140 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/__init__.py
+-rw-r--r--  2.0 unx     1077 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/__manifest__.py
+-rw-r--r--  2.0 unx      456 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/blacklist.py
+-rw-r--r--  2.0 unx    19987 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/compare.py
+-rw-r--r--  2.0 unx     8286 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/upgrade_log.py
+-rw-r--r--  2.0 unx    21146 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/i18n/es_AR.po
+-rw-r--r--  2.0 unx    18769 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/i18n/fr.po
+-rw-r--r--  2.0 unx    18533 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
+-rw-r--r--  2.0 unx      163 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/models/__init__.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/models/ir_module_module.py
+-rw-r--r--  2.0 unx    22565 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/models/upgrade_analysis.py
+-rw-r--r--  2.0 unx      536 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/models/upgrade_attribute.py
+-rw-r--r--  2.0 unx     3098 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py
+-rw-r--r--  2.0 unx     5998 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/models/upgrade_record.py
+-rw-r--r--  2.0 unx       65 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/__init__.py
+-rw-r--r--  2.0 unx     1835 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py
+-rw-r--r--  2.0 unx       66 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py
+-rw-r--r--  2.0 unx      270 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
+-rw-r--r--  2.0 unx      371 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
+-rw-r--r--  2.0 unx      259 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
+-rw-r--r--  2.0 unx       84 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
+-rw-r--r--  2.0 unx      729 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
+-rw-r--r--  2.0 unx       19 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py
+-rw-r--r--  2.0 unx     1589 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py
+-rw-r--r--  2.0 unx     1112 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
+-rw-r--r--  2.0 unx      397 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
+-rw-r--r--  2.0 unx      336 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.md
+-rw-r--r--  2.0 unx      677 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/readme/DESCRIPTION.md
+-rw-r--r--  2.0 unx      267 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/readme/ROADMAP.md
+-rw-r--r--  2.0 unx       69 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/readme/USAGE.md
+-rw-r--r--  2.0 unx      696 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/security/ir.model.access.csv
+-rw-r--r--  2.0 unx     9455 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/static/description/icon.png
+-rw-r--r--  2.0 unx    15067 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/static/description/index.html
+-rw-r--r--  2.0 unx      752 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako
+-rw-r--r--  2.0 unx       26 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/tests/__init__.py
+-rw-r--r--  2.0 unx     1787 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/tests/test_module.py
+-rw-r--r--  2.0 unx      200 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/views/menu.xml
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml
+-rw-r--r--  2.0 unx     2826 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml
+-rw-r--r--  2.0 unx     2814 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml
+-rw-r--r--  2.0 unx       82 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/wizards/__init__.py
+-rw-r--r--  2.0 unx     4527 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py
+-rw-r--r--  2.0 unx     4066 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py
+-rw-r--r--  2.0 unx     1919 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
+-rw-r--r--  2.0 unx     3454 b- defN 24-May-24 07:35 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
+-rw-r--r--  2.0 unx     5276 b- defN 24-May-24 07:35 odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       83 b- defN 24-May-24 07:35 odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-May-24 07:35 odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6021 b- defN 24-May-24 07:35 odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/RECORD
+54 files, 195902 bytes uncompressed, 55492 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -144,20 +144,20 @@
 
 Filename: odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/METADATA
+Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/WHEEL
+Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/top_level.txt
+Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/RECORD
+Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/upgrade_analysis/i18n/es_AR.po

```diff
@@ -223,24 +223,14 @@
 
 #. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_ir_module_module__is_odoo_module
 msgid "Is Odoo Module"
 msgstr "Es un Módulo de Odoo"
 
 #. module: upgrade_analysis
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record____last_update
-msgid "Last Modified on"
-msgstr "Última modificación en"
-
-#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__write_uid
 msgid "Last Updated by"
@@ -291,20 +281,24 @@
 #. module: upgrade_analysis
 #: model_terms:ir.ui.view,arch_db:upgrade_analysis.view_upgrade_record_search
 msgid "Modify Mode"
 msgstr "Modo de Modificación"
 
 #. module: upgrade_analysis
 #: model:ir.model,name:upgrade_analysis.model_ir_module_module
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__module_ids
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__module
 msgid "Module"
 msgstr "Módulo"
 
 #. module: upgrade_analysis
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__module_ids
+msgid "Modules"
+msgstr ""
+
+#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__module_qty
 msgid "Modules Quantity"
 msgstr "Cantidad de Módulos"
 
 #. module: upgrade_analysis
 #: model_terms:ir.ui.view,arch_db:upgrade_analysis.view_upgrade_generate_record_wizard_form
 msgid "Modules initialized and record created"
@@ -376,25 +370,14 @@
 "modifies an attribute of an existing field, set to Modify."
 msgstr ""
 "Establézcalo en Crear si se crea un campo recientemente en este módulo. Si "
 "este módulo modifica un atributo de un campo existente, configúrelo en "
 "Modificar."
 
 #. module: upgrade_analysis
-#: model:ir.model.fields,field_description:upgrade_analysis.field_ir_module_module__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__smart_search
-msgid "Smart Search"
-msgstr ""
-
-#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__state
 msgid "State"
 msgstr "Estado"
 
 #. module: upgrade_analysis
@@ -546,7 +529,10 @@
 msgid "upgrade Comparison Configs"
 msgstr "actualizar configuraciones de comparación"
 
 #. module: upgrade_analysis
 #: model:ir.actions.act_window,name:upgrade_analysis.action_upgrade_record_tree
 msgid "upgrade Records"
 msgstr "actualizar Registros"
+
+#~ msgid "Last Modified on"
+#~ msgstr "Última modificación en"
```

## odoo/addons/upgrade_analysis/i18n/fr.po

```diff
@@ -220,24 +220,14 @@
 
 #. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_ir_module_module__is_odoo_module
 msgid "Is Odoo Module"
 msgstr ""
 
 #. module: upgrade_analysis
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record____last_update
-msgid "Last Modified on"
-msgstr ""
-
-#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__write_uid
 msgid "Last Updated by"
@@ -288,20 +278,24 @@
 #. module: upgrade_analysis
 #: model_terms:ir.ui.view,arch_db:upgrade_analysis.view_upgrade_record_search
 msgid "Modify Mode"
 msgstr ""
 
 #. module: upgrade_analysis
 #: model:ir.model,name:upgrade_analysis.model_ir_module_module
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__module_ids
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__module
 msgid "Module"
 msgstr ""
 
 #. module: upgrade_analysis
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__module_ids
+msgid "Modules"
+msgstr ""
+
+#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__module_qty
 msgid "Modules Quantity"
 msgstr ""
 
 #. module: upgrade_analysis
 #: model_terms:ir.ui.view,arch_db:upgrade_analysis.view_upgrade_generate_record_wizard_form
 msgid "Modules initialized and record created"
@@ -370,25 +364,14 @@
 #: model:ir.model.fields,help:upgrade_analysis.field_upgrade_record__mode
 msgid ""
 "Set to Create if a field is newly created in this module. If this module "
 "modifies an attribute of an existing field, set to Modify."
 msgstr ""
 
 #. module: upgrade_analysis
-#: model:ir.model.fields,field_description:upgrade_analysis.field_ir_module_module__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__smart_search
-msgid "Smart Search"
-msgstr ""
-
-#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__state
 msgid "State"
 msgstr ""
 
 #. module: upgrade_analysis
```

## Comparing `odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/METADATA` & `odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addon-upgrade_analysis
-Version: 17.0.1.0.0.6
+Version: 17.0.1.0.0.7
 Requires-Python: >=3.10
 Requires-Dist: dataclasses
 Requires-Dist: mako
 Requires-Dist: odoo>=17.0a,<17.1dev
 Requires-Dist: odoorpc
 Requires-Dist: openupgradelib
 Summary: Performs a difference analysis between modules installed on two different Odoo instances
```

## Comparing `odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/RECORD` & `odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 odoo/addons/upgrade_analysis/README.rst,sha256=tn0jBATwQt-CmUTv6MpAQikvbDL29B0hHqy5Ea6okLI,4578
 odoo/addons/upgrade_analysis/__init__.py,sha256=1X8E6viDvX9QCI3au33OFkjFkJbFw6TazruSkrDurdI,140
 odoo/addons/upgrade_analysis/__manifest__.py,sha256=2TPFpeXvDNcWJ1V1EZyc6kNVAKu-7ZIwIKiBW4jiyXY,1077
 odoo/addons/upgrade_analysis/blacklist.py,sha256=h2b5VsBPF0Z6imWpZme37xZE-m0nmRdpzUbTWHW7u3E,456
 odoo/addons/upgrade_analysis/compare.py,sha256=r8S_JEwZFYwYqtS0AKK_c7jizG6Kg6fmSrspn0kafug,19987
 odoo/addons/upgrade_analysis/upgrade_log.py,sha256=POS59R1IbnrrMvKzWpcz1yNW_5oQ0skIhc6pDh8nruw,8286
-odoo/addons/upgrade_analysis/i18n/es_AR.po,sha256=fHZ_DD9rAwE5ecWSzlX3WMep0t3FG3I7Qsqnchq5f2Y,22496
-odoo/addons/upgrade_analysis/i18n/fr.po,sha256=uzNf1Vqaxcu3y6-CHg_IXUPFdNg6DHVOAB3mR75VDaY,20161
+odoo/addons/upgrade_analysis/i18n/es_AR.po,sha256=KV4WxHP5jjLw4vtCCdfinsjwNTor2iDOzT7FnbAzR8U,21146
+odoo/addons/upgrade_analysis/i18n/fr.po,sha256=XoF1oggOhjCA-ZX9IuMKGKBBxJdDdpbK0YAgATbJ0L4,18769
 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot,sha256=Hx2KXpgfF4Ui2Aj5W8_vZC9w5AMgRw5I8njKi4teWJE,18533
 odoo/addons/upgrade_analysis/models/__init__.py,sha256=V3z7qRHAST0ArkG6eGCgABdDHniOvY7Mcna8I4M5duk,163
 odoo/addons/upgrade_analysis/models/ir_module_module.py,sha256=Wy2bfWlulZ-ucpxh6flDgGcvCPBpeL1TztPCxW1x-9U,1031
 odoo/addons/upgrade_analysis/models/upgrade_analysis.py,sha256=nBDMvRAswBm283i9Ff5CHDuO74aIxJYNtu8sfl_zNO4,22565
 odoo/addons/upgrade_analysis/models/upgrade_attribute.py,sha256=j2K_dqArvAHThW51VWhiNSiyoy9g5BnPS01khhaaovw,536
 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py,sha256=2v-0S5vXoFZsL7e-wXlHdWdf3j5v222pYK5kKcbLCmk,3098
 odoo/addons/upgrade_analysis/models/upgrade_record.py,sha256=dAtwYng98TJJclE04KMwMd2nuGMbEZMuQvGnXcABHV0,5998
@@ -44,11 +44,11 @@
 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml,sha256=pBTVmGOGkohO1tguxKFXAWGHkrSVJdok3jjuhERcGa4,2826
 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml,sha256=oH7i44cTERaDYRRQzcYUOtRvntBrhJJ9bxPdpl91L7k,2814
 odoo/addons/upgrade_analysis/wizards/__init__.py,sha256=6973yn8jkeAaHm-ofIILbHUCB6KQ7RUMSDCK0Xk18xE,82
 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py,sha256=DTeLN_1rez_v82EA16H2Bsk4TGk9aA_n7Wn6_qQoKUE,4527
 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py,sha256=ysFWUHxBYO4HKGO4SzwD_Tq0rNr9YUlUv73APpyfIto,4066
 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml,sha256=BUYgXSoebkDkezLQirUJIZbZxHuU3-gesUtOZ1eP00I,1919
 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml,sha256=bKziKQUjgGfeXri_cj_0Vgkbj2M5I4IbX9xxlgoLEFI,3454
-odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/METADATA,sha256=oolP0nsBtOjHDi4kWyf1EIJWGq8tozU6qUMycl4kS3I,5276
-odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/WHEEL,sha256=8Rd4enx1PCuyDWP4SABqO5Fv8rpaknqp3VzjoFFLa6c,83
-odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/top_level.txt,sha256=QE6RBQ0QX5f4eFuUcGgU5Kbq1A_qJcDs-e_vpr6pmfU,4
-odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/RECORD,,
+odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/METADATA,sha256=U6mRzG2hAa_PoemqFj1FLKosTHUm6qqOrxP_5uefJFM,5276
+odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/WHEEL,sha256=8Rd4enx1PCuyDWP4SABqO5Fv8rpaknqp3VzjoFFLa6c,83
+odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/top_level.txt,sha256=QE6RBQ0QX5f4eFuUcGgU5Kbq1A_qJcDs-e_vpr6pmfU,4
+odoo_addon_upgrade_analysis-17.0.1.0.0.7.dist-info/RECORD,,
```

