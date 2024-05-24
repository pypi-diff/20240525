# Comparing `tmp/hnt_nf_jira_library-0.4.8.tar.gz` & `tmp/hnt_nf_jira_library-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.4.8.tar", last modified: Sat May  4 18:50:03 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.4.9.tar", last modified: Mon May  6 18:42:21 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.4.8.tar` & `hnt_nf_jira_library-0.4.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 18:50:03.885239 hnt_nf_jira_library-0.4.8/
--rw-rw-rw-   0        0        0      183 2024-05-04 18:50:03.884722 hnt_nf_jira_library-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-23 21:17:37.000000 hnt_nf_jira_library-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 18:50:03.858262 hnt_nf_jira_library-0.4.8/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      183 2024-05-04 18:50:03.000000 hnt_nf_jira_library-0.4.8/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2024-05-04 18:50:03.000000 hnt_nf_jira_library-0.4.8/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 18:50:03.000000 hnt_nf_jira_library-0.4.8/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-04 18:50:03.000000 hnt_nf_jira_library-0.4.8/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-04 18:50:03.000000 hnt_nf_jira_library-0.4.8/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 18:50:03.860387 hnt_nf_jira_library-0.4.8/nf_jira/
--rw-rw-rw-   0        0        0       41 2024-04-26 20:27:31.000000 hnt_nf_jira_library-0.4.8/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:50:03.879046 hnt_nf_jira_library-0.4.8/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-23 21:17:37.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      131 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:50:03.883689 hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4893 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     3672 2024-04-30 11:22:42.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2051 2024-05-04 18:32:46.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     7667 2024-04-30 11:22:42.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0      774 2024-04-26 20:18:01.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     3613 2024-05-04 18:32:46.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      593 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      480 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      793 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      419 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      485 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      460 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0     1167 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 12:03:57.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.8/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    16173 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.8/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-05-04 18:50:03.885239 hnt_nf_jira_library-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0      468 2024-05-04 18:47:36.000000 hnt_nf_jira_library-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:42:21.100917 hnt_nf_jira_library-0.4.9/
+-rw-rw-rw-   0        0        0      183 2024-05-06 18:42:21.100917 hnt_nf_jira_library-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2024-05-06 18:41:09.000000 hnt_nf_jira_library-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 18:42:21.069059 hnt_nf_jira_library-0.4.9/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      183 2024-05-06 18:42:20.000000 hnt_nf_jira_library-0.4.9/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2024-05-06 18:42:21.000000 hnt_nf_jira_library-0.4.9/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 18:42:20.000000 hnt_nf_jira_library-0.4.9/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-06 18:42:20.000000 hnt_nf_jira_library-0.4.9/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 18:42:20.000000 hnt_nf_jira_library-0.4.9/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 18:42:21.071060 hnt_nf_jira_library-0.4.9/nf_jira/
+-rw-rw-rw-   0        0        0       41 2024-04-26 20:27:31.000000 hnt_nf_jira_library-0.4.9/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:42:21.093462 hnt_nf_jira_library-0.4.9/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-23 21:17:37.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      131 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:42:21.099917 hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4893 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     3672 2024-04-30 11:22:42.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2051 2024-05-04 18:51:34.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     7667 2024-04-30 11:22:42.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0      774 2024-04-26 20:18:01.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     3613 2024-05-04 18:51:34.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      593 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      480 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0      198 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      793 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0      419 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      485 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      460 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0     1167 2024-05-01 13:25:21.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0      169 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 12:03:57.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.9/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    16230 2024-05-06 18:31:37.000000 hnt_nf_jira_library-0.4.9/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 18:42:21.100917 hnt_nf_jira_library-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      468 2024-05-06 18:32:37.000000 hnt_nf_jira_library-0.4.9/setup.py
```

### Comparing `hnt_nf_jira_library-0.4.8/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.4.9/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/form_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/helper.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/issue_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.8/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_library-0.4.9/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.8/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.4.9/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.8/nf_jira/entities/dados_basicos_fatura.py` & `hnt_nf_jira_library-0.4.9/nf_jira/entities/dados_basicos_fatura.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.8/nf_jira/entities/fatura.py` & `hnt_nf_jira_library-0.4.9/nf_jira/entities/fatura.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.8/nf_jira/entities/nota_pedido.py` & `hnt_nf_jira_library-0.4.9/nf_jira/entities/nota_pedido.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.8/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.4.9/nf_jira/wrapper_nf_jira.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,16 +336,16 @@
             leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'] is not None else None
             leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'] is not None else None
         elif issue['json_data'][COMPLEMENTO_DE_GÁS] is not None:
             leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'] is not None else None
             leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper()  if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'] is not None else None
 
         extra_ref = f"PERIODO: {leitura_anterior} A {leitura_atual}" if leitura_anterior is not None and leitura_atual is not None else None
-
-        return f"REF: {data_ref} {extra_ref}"
+        
+        return f"REF: {data_ref} {extra_ref}" if extra_ref is not None else f"REF: {data_ref}"
 
     def _get_issue_fields_by_keys(self, issue_key, form_template):
 
         form_jira_keys = self.FormJira.get_form_jira_keys(issue_key, form_template)
         form_fields    = self.FormJira.get_form_fields(issue_key, form_template)
         jira_fields    = self.IssueJira.get_issue_fields_data(issue_key)
         fields_by_jira_and_form = self.IssueFields.get_fields_by_form_and_jira(form_jira_keys, form_fields, jira_fields)
```

