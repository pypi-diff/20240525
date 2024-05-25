# Comparing `tmp/yeref-0.9.8.tar.gz` & `tmp/yeref-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.9.8.tar", last modified: Sun Feb  4 12:00:12 2024, max compression
+gzip compressed data, was "yeref-0.9.9.tar", last modified: Sun Feb  4 12:04:19 2024, max compression
```

## Comparing `yeref-0.9.8.tar` & `yeref-0.9.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-02-04 12:00:12.886230 yeref-0.9.8/
--rw-r--r--   0 mark       (501) staff       (20)       84 2024-02-04 12:00:12.884967 yeref-0.9.8/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2024-02-04 12:00:12.886451 yeref-0.9.8/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1122 2024-02-04 11:59:54.000000 yeref-0.9.8/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-02-04 12:00:12.868727 yeref-0.9.8/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       49 2023-12-19 18:48:18.000000 yeref-0.9.8/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)  1048942 2024-02-04 11:59:54.000000 yeref-0.9.8/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   485954 2024-01-31 20:33:39.000000 yeref-0.9.8/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-02-04 12:00:12.881229 yeref-0.9.8/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       84 2024-02-04 12:00:12.000000 yeref-0.9.8/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      169 2024-02-04 12:00:12.000000 yeref-0.9.8/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2024-02-04 12:00:12.000000 yeref-0.9.8/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2024-02-04 12:00:12.000000 yeref-0.9.8/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-02-04 12:04:19.068610 yeref-0.9.9/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2024-02-04 12:04:19.067079 yeref-0.9.9/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2024-02-04 12:04:19.068823 yeref-0.9.9/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1122 2024-02-04 12:04:04.000000 yeref-0.9.9/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-02-04 12:04:19.042066 yeref-0.9.9/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       49 2023-12-19 18:48:18.000000 yeref-0.9.9/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)  1048945 2024-02-04 12:04:04.000000 yeref-0.9.9/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   485954 2024-01-31 20:33:39.000000 yeref-0.9.9/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2024-02-04 12:04:19.065504 yeref-0.9.9/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2024-02-04 12:04:18.000000 yeref-0.9.9/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      169 2024-02-04 12:04:18.000000 yeref-0.9.9/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2024-02-04 12:04:18.000000 yeref-0.9.9/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2024-02-04 12:04:18.000000 yeref-0.9.9/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.9.8/setup.py` & `yeref-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='yeref',
-    version='0.9.8',
+    version='0.9.9',
     description='desc-f',
     author='john smith',
     packages=['yeref'],
     # install_requires=[
     #       "httplib2>=0.20.4",
     #       "moviepy>=1.0.3",
     #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.9.8/yeref/l_.py` & `yeref-0.9.9/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1493,15 +1493,15 @@
     'fr': "👩🏽‍💻 <b>Cliquez</b> [➕ Ajouter un bot]",
     'zh': "👩🏽‍💻 <b>点击</b> [➕ 添加机器人]",
     'ar': "👩🏽‍💻 <b>انقر</b> [➕ إضافة روبوت]",
 }
 
 # region commands
 l_bot_commands_handler = {
-    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>[<code>{1}</code>]\n\n<blockquote>/info    информация о боте\n/stat    статистика\n/status статус\n/on включение\n<code>/off</code>    выключение\n<code>/restart</code>   перезагрузка\n\n/parse   [premium|promo|utm|old|POST_ID]\n/promo    промокод\n/short    описание профиля¹²⁰\n/desc  описание бота⁵¹²\n/admin    администраторы\n/ban [id/@username] список\n/unban  разбан\n/transfer   передача admin-прав</blockquote>\n\n💨 <b>Подписка</b>: <i>{2}</i>",
+    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b> [<code>{1}</code>]\n\n<blockquote>/info    информация о боте\n/stat    статистика\n/status статус\n/on включение\n<code>/off</code>    выключение\n<code>/restart</code>   перезагрузка\n\n/parse   [premium|promo|utm|old|POST_ID]\n/promo    промокод\n/short    описание профиля¹²⁰\n/desc  описание бота⁵¹²\n/admin    администраторы\n/ban [id/@username] список\n/unban  разбан\n/transfer   передача admin-прав</blockquote>\n\n💨 <b>Подписка</b>: <i>{2}</i>",
     'en': "⚙️ <b>Commands</b> /cmd for <b>@{0}</b>\n\n/info <i>bot information</i>\n/stat <i>statistics</i >\n/status <i>status</i>\n/on <i>on</i>\n<code>/off</code> <i>off</i>\n<code>/ restart</code> <i>restart</i>\n\n/parse [premium|promo|utm|old|POST_ID]\n/promo <i>promo code</i>\n/admin <i>administrators </i>\n/ban [id/ @username] <i>list</i>\n/unban <i>unban</i>\n/transfer <i>transfer of admin rights</i>\ n\n💨 <b>Subscription</b>: <i>{1}</i>",
     'es': "⚙️ <b>Comandos</b> /cmd para <b>@{0}</b>\n\n/info <i>información del bot</i>\n/stat <i>estadísticas</i >\n/status <i>estado</i>\n/on <i>on</i>\n<code>/off</code> <i>off</i>\n<code>/reiniciar </code> <i>reiniciar</i>\n\n/parse [premium|promo|utm|old|POST_ID]\n/promo <i>código de promoción</i>\n/admin <i>administradores </i>\n/ban [id/ @username] <i>list</i>\n/unban <i>unban</i>\n/transfer <i>transferencia de derechos de administrador</i>\ n\n💨 <b>Suscripción</b>: <i>{1}</i>",
     'fr': "⚙️ <b>Commandes</b> /cmd pour <b>@{0}</b>\n\n/info <i>informations sur le robot</i>\n/stat <i>statistiques</i >\n/statut <i>statut</i>\n/on <i>on</i>\n<code>/off</code> <i>off</i>\n<code>/ redémarrage </code> <i>redémarrer</i>\n\n/parse [premium|promo|utm|old|POST_ID]\n/promo <i>code promo</i>\n/admin <i>administrateurs </i>\n/ban [id/ @username] <i>list</i>\n/unban <i>unban</i>\n/transfer <i>transfert des droits d'administrateur</i>\ n\n💨 <b>Abonnement</b> : <i>{1}</i>",
     'zh': "⚙️ <b>命令</b> /cmd for <b>@{0}</b>\n\n/info <i>机器人信息</i>\n/stat <i>统计</i>\n/status <i>状态</i>\n/on <i>开</i>\n<code>/off</code> <i>关</i>\n<code>/重启</code> <i>重新启动</i>\n\n/parse [premium|promo|utm|old|POST_ID]\n/promo <i>促销代码</i>\n/admin <i>管理员</i>\n/ban [id/ @username] <i>列表</i>\n/unban <i>解禁</i>\n/transfer <i>转让管理权限</i>\ n\n💨 <b>订阅</b>：<i>{1}</i>",
     'ar': "⚙️ <b>الأوامر</b> /cmd لـ <b>@{0}</b>\n\n/info <i>معلومات الروبوت</i>\n/stat <i>الإحصائيات</i >\n/status <i>status</i>\n/on <i>on</i>\n<code>/off</code> <i>off</i>\n<code>/ Restart </code> <i>إعادة التشغيل</i>\n\n/parse [premium|promo|utm|old|POST_ID]\n/promo <i>الرمز الترويجي</i>\n/admin <i>المسؤولين </i>\n/ban [id/ @username] <i>list</i>\n/unban <i>unban</i>\n/transfer <i>نقل حقوق المسؤول</i>\n\n💨 <b>الاشتراك</b>: <i>{1}</i>",
 }
 l_bot_info_handler = {
@@ -6030,15 +6030,15 @@
     'zh': "👮🏽 要<i>检查订阅</i>，您需要使用以下命令添加频道：\n\n/channel LINK TO CHANNEL",
     'ar': "👮🏽 <i>للتحقق من الاشتراك</i>، يلزمك إضافة قناة باستخدام الأمر:\n\n/channel LINK TO CHANNEL",
 }
 
 
 # region commands
 l_chn_commands_handler = {
-    'ru': "⚙️ <b>Команды</b> /cmd для [<b>{0}</b>] {1}[<code>{2}</code>]\n\n<blockquote>/info   информация о канале\n/stat  статистика\n\n/parse    [1] база подписчиков/лайков\n/random    [1] рандомный лайкнувший пост #1\n/podcast 1 1  анонс видео-подкаста\n<code>/clean</code>   очистка от deleted/scam-аккаунтов и по [<b>🕵🏽 Авто-бан</b>] правилам\n/delete   <code>FROM TO</code>    удаление за период\n/channel NAME   канал проверки подписки\n/transfer  передача admin-прав</blockquote>\n\n💨 <b>Подписка</b>: <i>{3}</i>",
+    'ru': "⚙️ <b>Команды</b> /cmd для [<b>{0}</b>] {1} [<code>{2}</code>]\n\n<blockquote>/info   информация о канале\n/stat  статистика\n\n/parse    [1] база подписчиков/лайков\n/random    [1] рандомный лайкнувший пост #1\n/podcast 1 1  анонс видео-подкаста\n<code>/clean</code>   очистка от deleted/scam-аккаунтов и по [<b>🕵🏽 Авто-бан</b>] правилам\n/delete   <code>FROM TO</code>    удаление за период\n/channel NAME   канал проверки подписки\n/transfer  передача admin-прав</blockquote>\n\n💨 <b>Подписка</b>: <i>{3}</i>",
     'en': "⚙️ <b>Commands</b> /cmd for [<b>{0}</b>] {1}\n\n/info <i>channel information</i>\n/stat <i> statistics</i>\n\n/parse [1] <i>subscriber/click base</i>\n/podcast 1 1 <i>video podcast announcement</i>\n<code>/clean< /code> <i>clearing deleted/scam accounts and [🕵🏽 Auto-ban] rules</i>\n/delete <code>FROM TO</code> <i>delete for a period</i>\ n/channel NAME <i>subscription verification channel</i>\n/transfer <i>transfer of admin rights</i>\n\n💨 <b>Subscription</b>: <i>{2}< /i>",
     'es': "⚙️ <b>Comandos</b> /cmd para [<b>{0}</b>] {1}\n\n/info <i>información del canal</i>\n/stat <i> estadísticas </i>\n\n/parse [1] <i>base de suscriptores/clics</i>\n/podcast 1 1 <i>anuncio de podcast en vídeo</i>\n<code>/clean< /code > <i>borrar cuentas eliminadas/estafas y reglas de [🕵🏽 Prohibición automática]</i>\n/eliminar <code>DE HASTA</code> <i>eliminar por un período</i>\ n/canal NOMBRE <i>canal de verificación de suscripción</i>\n/transfer <i>transferencia de derechos de administrador</i>\n\n💨 <b>Suscripción</b>: <i>{2}< /i>",
     'fr': "⚙️ <b>Commandes</b> /cmd pour [<b>{0}</b>] {1}\n\n/info <i>informations sur la chaîne</i>\n/stat <i> statistiques </i>\n\n/parse [1] <i>abonné/clic de base</i>\n/podcast 1 1 <i>annonce de podcast vidéo</i>\n<code>/clean< /code > <i>effacer les comptes supprimés/arnaqueurs et les règles de [🕵🏽 Auto-ban]</i>\n/supprimer <code>FROM TO</code> <i>supprimer pendant une période</i>\ n/canal NOM <i>canal de vérification d'abonnement</i>\n/transfert <i>transfert des droits d'administrateur</i>\n\n💨 <b>Abonnement</b> : <i>{2}< /i>",
     'zh': "⚙️ <b>命令</b> /cmd 用于 [<b>{0}</b>] {1}\n\n/info <i>频道信息</i>\n/stat <i> 统计信息</i>\n\n/parse [1] <i>订阅者/点击量</i>\n/podcast 1 1 <i>视频播客公告</i>\n<code>/clean</code > <i>清除已删除/诈骗帐户和[🕵🏽自动禁止]规则</i>\n/delete <code>FROM TO</code> <i>删除一段时间</i>\n/channel NAME <i>订阅验证通道</i>\n/transfer <i>管理权限转让</i>\n\n💨 <b>订阅</b>：<i>{2}</i>",
     'ar': "⚙️ <b>الأوامر</b> /cmd لإحصائيات [<b>{0}</b>] {1}\n\n/info <i>معلومات القناة</i>\n/stat <i> </i>\n\n/parse [1] <i>قاعدة المشترك/النقر</i>\n/podcast 1 1 <i>إعلان بودكاست فيديو</i>\n<code>/clean< /code > <i>مسح الحسابات المحذوفة/المحتالة وقواعد [🕵🏽 الحظر التلقائي]</i>\n/حذف <code>من إلى</code> <i>حذف لفترة</i>\n/channel الاسم <i>قناة التحقق من الاشتراك</i>\n/transfer <i>نقل حقوق المسؤول</i>\n\n💨 <b>الاشتراك</b>: <i>{2}< /i>",
 }
 l_update_text = {
@@ -7150,15 +7150,15 @@
     'ar': "👮🏽 <i>للتحقق من الاشتراك</i>، يلزمك إضافة قناة باستخدام الأمر:\n\n/channel LINK TO CHANNEL",
 }
 # endregion
 
 
 # region commands
 l_grp_commands_handler = {
-    'ru': "⚙️ <b>Команды</b> /cmd для [<b>{0}</b>] {1}[<code>{2}</code>]\n\n<b>⛏ Команды в @{3}</b>\n\n<blockquote>/info    информация о группе\n/stat  статистика\n/parse  [all|old|premium|active|online|'post_id']\n/random   [1]    рандомный лайкнувший пост #1\n/podcast 1 1  анонс видео-подкаста\n<code>/clean</code>   очистка от deleted/scam-аккаунтов и по [<b>🕵🏽 Авто-бан</b>] правилам\n/delete   <code>FROM TO</code>    удаление за период\n/work   часы работы группы\n/transfer   передача admin-прав</blockquote>\n\n<b>⛏ Команды администраторов</b>\n\n<blockquote>/ban 5m|1h|10d  удаление на время\n/unban\n/mute 5m|1h|10d  ограничение на время\n/unmute\n/warn+сообщ  предупреждение\n/status\n/karma  [+|-]\n/tag+сообщ  случайное @упоминание\n/stop    добавить стоп-слово\n/channel NAME  канал проверки подписки\n/button NAME   имя кнопки входного контроля\n/delay MIN    задержка 1го сообщ в min\n/flood NUM    количество сообщ для флуд-режима\n/len MAX  max-длина сообщ\n/timer SEC задержка 1го комментария в сек</blockquote>\n\n<b>⛏ Команды пользователей</b>\n\n<blockquote>/help  вывод команд\n/rules    правила группы\n/report сообщить о нарушении\n/happy    получить радость\n/thanks   поблагодарить\n/birthday    поздравить</blockquote>\n\n💨 <b>Подписка</b>: <i>{4}</i>",
+    'ru': "⚙️ <b>Команды</b> /cmd для [<b>{0}</b>] {1} [<code>{2}</code>]\n\n<b>⛏ Команды в @{3}</b>\n\n<blockquote>/info    информация о группе\n/stat  статистика\n/parse  [all|old|premium|active|online|'post_id']\n/random   [1]    рандомный лайкнувший пост #1\n/podcast 1 1  анонс видео-подкаста\n<code>/clean</code>   очистка от deleted/scam-аккаунтов и по [<b>🕵🏽 Авто-бан</b>] правилам\n/delete   <code>FROM TO</code>    удаление за период\n/work   часы работы группы\n/transfer   передача admin-прав</blockquote>\n\n<b>⛏ Команды администраторов</b>\n\n<blockquote>/ban 5m|1h|10d  удаление на время\n/unban\n/mute 5m|1h|10d  ограничение на время\n/unmute\n/warn+сообщ  предупреждение\n/status\n/karma  [+|-]\n/tag+сообщ  случайное @упоминание\n/stop    добавить стоп-слово\n/channel NAME  канал проверки подписки\n/button NAME   имя кнопки входного контроля\n/delay MIN    задержка 1го сообщ в min\n/flood NUM    количество сообщ для флуд-режима\n/len MAX  max-длина сообщ\n/timer SEC задержка 1го комментария в сек</blockquote>\n\n<b>⛏ Команды пользователей</b>\n\n<blockquote>/help  вывод команд\n/rules    правила группы\n/report сообщить о нарушении\n/happy    получить радость\n/thanks   поблагодарить\n/birthday    поздравить</blockquote>\n\n💨 <b>Подписка</b>: <i>{4}</i>",
     'en': "⚙️ <b>Commands</b> /cmd for [<b>{0}</b>] {1}\n\n<b>⛏ Commands in @{2}</b>\n/info < i>group information</i>\n/stat <i>statistics</i>\n/parse <i>[all|old|premium|active|online|'post_id']</i>\n/ podcast 1 1 <i>announcement of a video podcast</i>\n<code>/clean</code> <i>cleaning of deleted/scam accounts and [🕵🏽 Auto-ban] rules</i>\n/delete <code>FROM TO</code> <i>delete for a period</i>\n/work <i>group work hours</i>\n/transfer <i>transfer of admin rights</i>\n\n<b>⛏ Administrator commands</b>\n/ban 5m|1h|10d <i>temporary removal</i>\n/unban\n/mute 5m|1h|10d <i>restriction for a while</i>\n/unmute\n/warn+message <i>warning</i>\n/status\n/karma [+|-]\n/tag+message <i> @tager random-accounts</i>\n/stop <i>add a safe word</i>\n/channel NAME <i>subscription verification channel</i>\n/button NAME <i>input control button name</i >\n/delay MIN <i>delay of the 1st message in min</i>\n/flood NUM <i>number of messages for flood mode</i>\n/len MAX <i>max message length</ i>\n/timer SEC <i>delay of the 1st comment in sec</i>\n\n<b>⛏ User commands</b>\n/help <i>command output</i>\n/rules <i>group rules</i>\n/report <i>report violation</i>\n/happy <i>get joy</i>\n/thanks <i>thank</i>\n/birthday <i>congratulate</i>\n\n💨 <b>Subscription</b>: <i>{3}</i>",
     'es': "⚙️ <b>Comandos</b> /cmd para [<b>{0}</b>] {1}\n\n<b>⛏ Comandos en @{2}</b>\n/info < i>información del grupo</i>\n/stat <i>estadísticas</i>\n/parse <i>[all|old|premium|active|online|'post_id']</i>\n/ podcast 1 1 <i>anuncio de un podcast de vídeo</i>\n<code>/clean</code> <i>limpieza de cuentas eliminadas/estafas y reglas de [🕵🏽 Auto-ban]</i>\n/ eliminar <code>DE HASTA</code> <i>eliminar por un período</i>\n/work <i>horas de trabajo grupal</i>\n/transfer <i>transferencia de derechos de administrador</i>\n\n<b>⛏ Comandos de administrador</b>\n/ban 5m|1h|10d <i>eliminación temporal</i>\n/unban\n/mute 5m|1h|10d <i>restricción para un rato</i>\n/activar silencio\n/warn+mensaje <i>advertencia</i>\n/status\n/karma [+|-]\n/tag+mensaje <i> @tager aleatorio-cuentas</i>\n/stop <i>añadir una palabra segura</i>\n/channel NAME <i>canal de verificación de suscripción</i>\n/button NAME <i>ingrese el nombre del botón de control</i >\n/delay MIN <i>retraso del 1er mensaje en min</i>\n/flood NUM <i>número de mensajes para el modo de inundación</i>\n/len MAX <i>longitud máxima del mensaje< / i>\n/timer SEC <i>retraso del 1er comentario en segundos</i>\n\n<b>⛏ Comandos de usuario</b>\n/help <i>salida del comando</i>\ n/rules <i>reglas del grupo</i>\n/report <i>informar infracción</i>\n/feliz <i>obtener alegría</i>\n/gracias <i>gracias</i>\n/cumpleaños <i>felicitaciones</i>\n\n💨 <b>Suscripción</b>: <i>{3}</i>",
     'fr': "⚙️ <b>Commandes</b> /cmd pour [<b>{0}</b>] {1}\n\n<b>⛏ Commandes dans @{2}</b>\n/info < i>informations sur le groupe</i>\n/stat <i>statistiques</i>\n/parse <i>[all|old|premium|active|online|'post_id']</i>\n/ podcast 1 1 <i>annonce d'un podcast vidéo</i>\n<code>/clean</code> <i>nettoyage des comptes supprimés/arnaqueurs et règles de [🕵🏽 Auto-ban]</i>\n/ supprimer <code>DE VERS</code> <i>supprimer pour une période</i>\n/travail <i>heures de travail en groupe</i>\n/transfert <i>transfert des droits d'administrateur</i>\n\n<b>⛏ Commandes administrateur</b>\n/ban 5m|1h|10d <i>suppression temporaire</i>\n/unban\n/mute 5m|1h|10d <i>restriction pour un moment</i>\n/activer le son\n/warn+message <i>avertissement</i>\n/status\n/karma [+|-]\n/tag+message <i> @tager random-comptes</i>\n/stop <i>ajouter un mot de sécurité</i>\n/nom du canal <i>canal de vérification d'abonnement</i>\n/nom du bouton <i>nom du bouton de contrôle de saisie</i >\n/delay MIN <i>délai du 1er message en min</i>\n/flood NUM <i>nombre de messages pour le mode Flood</i>\n/len MAX <i>longueur max du message< / i>\n/timer SEC <i>délai du 1er commentaire en sec</i>\n\n<b>⛏ Commandes utilisateur</b>\n/help <i>sortie de commande</i>\ n/règles <i>règles de groupe</i>\n/rapport <i>signaler une violation</i>\n/heureux <i>prenez de la joie</i>\n/merci <i>merci</i>\n/anniversaire <i>féliciter</i>\n\n💨 <b>Abonnement</b> : <i>{3}</i>",
     'zh': "⚙️ <b>命令</b> /cmd for [<b>{0}</b>] {1}\n\n<b>⛏ @{2}</b>\n/info 中的命令 < i>群组信息</i>\n/stat <i>统计</i>\n/parse <i>[all|old|premium|active|online|'post_id']</i>\n/ podcast 1 1 <i>视频播客公告</i>\n<code>/clean</code> <i>清理已删除/诈骗帐户和[🕵🏽自动禁止]规则</i>\n/删除<code>从到</code> <i>删除一段时间</i>\n/work <i>小组工作时间</i>\n/transfer <i>管理权限转让</i>\n\n<b>⛏ 管理员命令</b>\n/ban 5m|1h|10d <i>临时删除</i>\n/unban\n/mute 5m|1h|10d <i>限制一会儿</i>\n/unmute\n/warn+message <i>警告</i>\n/status\n/karma [+|-]\n/tag+message <i> @tager random-帐户</i>\n/stop <i>添加安全词</i>\n/channel NAME <i>订阅验证通道</i>\n/button NAME <i>输入控制按钮名称</i >\n/delay MIN <i>第一条消息的延迟时间</i>\n/flood NUM <i>洪水模式的消息数量</i>\n/len MAX <i>最大消息长度< / i>\n/timer SEC <i>以秒为单位延迟第一个注释</i>\n\n<b>⛏ 用户命令</b>\n/help <i>命令输出</i>\ n/rules<i>群组规则</i>\n/report<i>举报违规行为</i>\n/happy<i>获得快乐</i>\n/thanks<i>感谢</i>\n/生日<i>恭喜</i>\n\n💨<b>订阅</b>：<i>{3}</i>",
     'ar': "⚙️ <b>الأوامر</b> /cmd لـ [<b>{0}</b>] {1}\n\n<b>⛏ الأوامر في @{2}</b>\n/info <<i>معلومات المجموعة</i>\n/stat <i>الإحصائيات</i>\n/parse <i>[all|old|premium|active|online|'post_id']</i>\n/ podcast 1 1 <i>إعلان عن بودكاست فيديو</i>\n<code>/clean</code> <i>تنظيف الحسابات المحذوفة/المحتالة وقواعد [🕵🏽 الحظر التلقائي]</i>\n/ حذف <code>من إلى</code> <i>حذف لفترة</i>\n/العمل <i>ساعات عمل جماعية</i>\n/نقل <i>نقل حقوق المسؤول</i>\n\n<b>⛏ أوامر المسؤول</b>\n/ban 5m|1h|10d <i>الإزالة المؤقتة</i>\n/unban\n/mute 5m|1h|10d <i>تقييد لـ فترة</i>\n/unmute\n/warn+message <i>warning</i>\n/status\n/karma [+|-]\n/tag+message <i> @tager عشوائي-الحسابات</i>\n/stop <i>إضافة كلمة آمنة</i>\n/channel NAME <i>قناة التحقق من الاشتراك</i>\n/button NAME <i>اسم زر التحكم في الإدخال</i >\n/delay MIN <i>تأخير الرسالة الأولى في الحد الأدنى</i>\n/flood NUM <i>عدد الرسائل في وضع الفيضان</i>\n/len MAX <i>الحد الأقصى لطول الرسالة< /<i>\n/timer SEC <i>تأخير التعليق الأول في ثانية</i>\n\n<b>⛏ أوامر المستخدم</b>\n/help <i>مخرج الأمر</i>\n/rules <i>قواعد المجموعة</i>\n/report <i>الإبلاغ عن انتهاك</i>\n/happy <i>استمتع</i>\n/شكرًا <i>شكرًا</i>\n/عيد الميلاد <i>تهنئة</i>\n\n💨 <b>الاشتراك</b>: <i>{3}</i>",
 }
 l_update_handler00 = {
```

### Comparing `yeref-0.9.8/yeref/yeref.py` & `yeref-0.9.9/yeref/yeref.py`

 * *Files identical despite different names*

