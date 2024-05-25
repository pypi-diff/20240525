# Comparing `tmp/mail-parser-reply-1.25.tar.gz` & `tmp/mail_parser_reply-1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/alfons/Documents/PycharmProjects/mail-parser/dist/.tmp-8xrl29as/mail-parser-reply-1.25.tar", last modified: Sun Nov 19 00:38:55 2023, max compression
+gzip compressed data, was "/Users/alfons/Documents/PycharmProjects/mail-parser/dist/.tmp-uzk_1upq/mail_parser_reply-1.26.tar", last modified: Sat May 25 10:22:29 2024, max compression
```

## Comparing `mail-parser-reply-1.25.tar` & `mail_parser_reply-1.26.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alfons     (501) staff       (20)        0 2023-11-19 00:38:55.241851 mail-parser-reply-1.25/
--rw-r--r--   0 alfons     (501) staff       (20)     1088 2023-01-04 17:13:31.000000 mail-parser-reply-1.25/LICENSE
--rw-r--r--   0 alfons     (501) staff       (20)       34 2023-01-04 17:08:44.000000 mail-parser-reply-1.25/MANIFEST.in
--rw-r--r--   0 alfons     (501) staff       (20)     4573 2023-11-19 00:38:55.241596 mail-parser-reply-1.25/PKG-INFO
--rw-r--r--   0 alfons     (501) staff       (20)     3895 2023-11-19 00:31:50.000000 mail-parser-reply-1.25/README.md
-drwxr-xr-x   0 alfons     (501) staff       (20)        0 2023-11-19 00:38:55.239815 mail-parser-reply-1.25/mail_parser_reply.egg-info/
--rw-r--r--   0 alfons     (501) staff       (20)     4573 2023-11-19 00:38:55.000000 mail-parser-reply-1.25/mail_parser_reply.egg-info/PKG-INFO
--rw-r--r--   0 alfons     (501) staff       (20)      348 2023-11-19 00:38:55.000000 mail-parser-reply-1.25/mail_parser_reply.egg-info/SOURCES.txt
--rw-r--r--   0 alfons     (501) staff       (20)        1 2023-11-19 00:38:55.000000 mail-parser-reply-1.25/mail_parser_reply.egg-info/dependency_links.txt
--rw-r--r--   0 alfons     (501) staff       (20)       17 2023-11-19 00:38:55.000000 mail-parser-reply-1.25/mail_parser_reply.egg-info/top_level.txt
-drwxr-xr-x   0 alfons     (501) staff       (20)        0 2023-11-19 00:38:55.240997 mail-parser-reply-1.25/mailparser_reply/
--rw-r--r--   0 alfons     (501) staff       (20)       63 2023-01-04 17:04:50.000000 mail-parser-reply-1.25/mailparser_reply/__init__.py
--rw-r--r--   0 alfons     (501) staff       (20)     5579 2023-11-19 00:27:57.000000 mail-parser-reply-1.25/mailparser_reply/constants.py
--rw-r--r--   0 alfons     (501) staff       (20)    11074 2023-02-21 18:58:08.000000 mail-parser-reply-1.25/mailparser_reply/parser.py
--rw-r--r--   0 alfons     (501) staff       (20)       17 2023-11-19 00:28:17.000000 mail-parser-reply-1.25/mailparser_reply/version.py
--rw-r--r--   0 alfons     (501) staff       (20)       38 2023-11-19 00:38:55.241910 mail-parser-reply-1.25/setup.cfg
--rw-r--r--   0 alfons     (501) staff       (20)     1205 2023-01-05 23:45:34.000000 mail-parser-reply-1.25/setup.py
-drwxr-xr-x   0 alfons     (501) staff       (20)        0 2023-11-19 00:38:55.241142 mail-parser-reply-1.25/test/
--rw-r--r--   0 alfons     (501) staff       (20)     7440 2023-11-19 00:34:07.000000 mail-parser-reply-1.25/test/test_email_reply_parser.py
+drwxr-xr-x   0 alfons     (501) staff       (20)        0 2024-05-25 10:22:29.241873 mail_parser_reply-1.26/
+-rw-r--r--   0 alfons     (501) staff       (20)     1088 2023-01-04 17:13:31.000000 mail_parser_reply-1.26/LICENSE
+-rw-r--r--   0 alfons     (501) staff       (20)       34 2023-01-04 17:08:44.000000 mail_parser_reply-1.26/MANIFEST.in
+-rw-r--r--   0 alfons     (501) staff       (20)     4629 2024-05-25 10:22:29.241638 mail_parser_reply-1.26/PKG-INFO
+-rw-r--r--   0 alfons     (501) staff       (20)     3933 2024-05-25 10:15:56.000000 mail_parser_reply-1.26/README.md
+drwxr-xr-x   0 alfons     (501) staff       (20)        0 2024-05-25 10:22:29.241369 mail_parser_reply-1.26/mail_parser_reply.egg-info/
+-rw-r--r--   0 alfons     (501) staff       (20)     4629 2024-05-25 10:22:29.000000 mail_parser_reply-1.26/mail_parser_reply.egg-info/PKG-INFO
+-rw-r--r--   0 alfons     (501) staff       (20)      348 2024-05-25 10:22:29.000000 mail_parser_reply-1.26/mail_parser_reply.egg-info/SOURCES.txt
+-rw-r--r--   0 alfons     (501) staff       (20)        1 2024-05-25 10:22:29.000000 mail_parser_reply-1.26/mail_parser_reply.egg-info/dependency_links.txt
+-rw-r--r--   0 alfons     (501) staff       (20)       17 2024-05-25 10:22:29.000000 mail_parser_reply-1.26/mail_parser_reply.egg-info/top_level.txt
+drwxr-xr-x   0 alfons     (501) staff       (20)        0 2024-05-25 10:22:29.240635 mail_parser_reply-1.26/mailparser_reply/
+-rw-r--r--   0 alfons     (501) staff       (20)       63 2023-01-04 17:04:50.000000 mail_parser_reply-1.26/mailparser_reply/__init__.py
+-rw-r--r--   0 alfons     (501) staff       (20)     6223 2024-05-25 10:16:32.000000 mail_parser_reply-1.26/mailparser_reply/constants.py
+-rw-r--r--   0 alfons     (501) staff       (20)    11073 2024-05-25 10:15:56.000000 mail_parser_reply-1.26/mailparser_reply/parser.py
+-rw-r--r--   0 alfons     (501) staff       (20)       17 2024-05-25 10:15:56.000000 mail_parser_reply-1.26/mailparser_reply/version.py
+-rw-r--r--   0 alfons     (501) staff       (20)       38 2024-05-25 10:22:29.241921 mail_parser_reply-1.26/setup.cfg
+-rw-r--r--   0 alfons     (501) staff       (20)     1223 2023-11-19 12:08:02.000000 mail_parser_reply-1.26/setup.py
+drwxr-xr-x   0 alfons     (501) staff       (20)        0 2024-05-25 10:22:29.240885 mail_parser_reply-1.26/test/
+-rw-r--r--   0 alfons     (501) staff       (20)     8729 2024-05-25 10:15:56.000000 mail_parser_reply-1.26/test/test_email_reply_parser.py
```

### Comparing `mail-parser-reply-1.25/LICENSE` & `mail_parser_reply-1.26/LICENSE`

 * *Files identical despite different names*

### Comparing `mail-parser-reply-1.25/PKG-INFO` & `mail_parser_reply-1.26/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mail-parser-reply
-Version: 1.25
+Version: 1.26
 Summary: 📧 Email reply parser library for Python with multi-language support
 Home-page: https://github.com/alfonsrv/mail-parser-reply
 Author: Alfons R.
-Author-email: alfonsrv@pm.me
+Author-email: alfonsrv@protonmail.com
 Maintainer: Alfons R.
-Maintainer-email: alfonsrv@pm.me
+Maintainer-email: alfonsrv@protonmail.com
 License: MIT
 Keywords: mail,email,parser
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 ### Multi-language email reply parsing for international environments 🌍
 
 Mail clients handle reply formatting differently, making reliable parsing difficult. Thank god we have 
 [standards](https://xkcd.com/927/).  This library splits *text-based* emails into separate replies based on common 
 headers produced by different, multilingual clients usually indicating separation.
 
 Replies can either present the whole mail message body, or strip headers, signatures and common disclaimers if required. 
-Currently supported languages are: English (`en`), German (`de`), French (`fr`), Italian (`it`) and Japanese (`ja`) – 
+Currently supported languages are: English (`en`), German (`de`), French (`fr`), Italian (`it`), Japanese (`ja`), Polish (`pl`) – 
 adding more languages is quite easy.
 
 This is an improved Python implementation of GitHub's Ruby-based [email_reply_parser](https://github.com/github/email_reply_parser/) 
 and an adaptation of Zapier's [email-reply-parser](https://github.com/zapier/email-reply-parser) which both split the 
 mails in fragments instead of distinct replies. They also only support English.
 
 
@@ -95,23 +95,24 @@
 
 *Or* get only the latest reply using:
 
 ```python
 latest_reply = EmailReplyParser(languages=languages).parse_reply(text=mail_body)
 ```
 
+
 ### Parser API
 
 ```
 EmailMessage.text:              Mail body
 EmailMessage.languages:         Languages to use for parsing headers
 EmailMessage.replies:           List of EmailReply; single parsed replies
 EmailMessage.include_english:   Always include English language for parsing
 EmailMessage.default_language:  Default language to use if language dictionary 
-                                doesn't include
+                                doesn't include any other language codes
 
 EmailMessage.HEADER_REGEX:      RegEx for identifying headers, separating mails
 EmailMessage.SIGNATURE_REGEX:   RegEx for identifying signatures
 EmailMessage.DISCLAIMERS_REGEX: RegEx for identifying disclaimers
 
 EmailMessage.read(): Parse EmailMessage.text to EmailReply which are then stored 
                      in EmailMessage.replies
```

### Comparing `mail-parser-reply-1.25/README.md` & `mail_parser_reply-1.26/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ### Multi-language email reply parsing for international environments 🌍
 
 Mail clients handle reply formatting differently, making reliable parsing difficult. Thank god we have 
 [standards](https://xkcd.com/927/).  This library splits *text-based* emails into separate replies based on common 
 headers produced by different, multilingual clients usually indicating separation.
 
 Replies can either present the whole mail message body, or strip headers, signatures and common disclaimers if required. 
-Currently supported languages are: English (`en`), German (`de`), French (`fr`), Italian (`it`) and Japanese (`ja`) – 
+Currently supported languages are: English (`en`), German (`de`), French (`fr`), Italian (`it`), Japanese (`ja`), Polish (`pl`) – 
 adding more languages is quite easy.
 
 This is an improved Python implementation of GitHub's Ruby-based [email_reply_parser](https://github.com/github/email_reply_parser/) 
 and an adaptation of Zapier's [email-reply-parser](https://github.com/zapier/email-reply-parser) which both split the 
 mails in fragments instead of distinct replies. They also only support English.
 
 
@@ -75,23 +75,24 @@
 
 *Or* get only the latest reply using:
 
 ```python
 latest_reply = EmailReplyParser(languages=languages).parse_reply(text=mail_body)
 ```
 
+
 ### Parser API
 
 ```
 EmailMessage.text:              Mail body
 EmailMessage.languages:         Languages to use for parsing headers
 EmailMessage.replies:           List of EmailReply; single parsed replies
 EmailMessage.include_english:   Always include English language for parsing
 EmailMessage.default_language:  Default language to use if language dictionary 
-                                doesn't include
+                                doesn't include any other language codes
 
 EmailMessage.HEADER_REGEX:      RegEx for identifying headers, separating mails
 EmailMessage.SIGNATURE_REGEX:   RegEx for identifying signatures
 EmailMessage.DISCLAIMERS_REGEX: RegEx for identifying disclaimers
 
 EmailMessage.read(): Parse EmailMessage.text to EmailReply which are then stored 
                      in EmailMessage.replies
```

### Comparing `mail-parser-reply-1.25/mail_parser_reply.egg-info/PKG-INFO` & `mail_parser_reply-1.26/mail_parser_reply.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mail-parser-reply
-Version: 1.25
+Version: 1.26
 Summary: 📧 Email reply parser library for Python with multi-language support
 Home-page: https://github.com/alfonsrv/mail-parser-reply
 Author: Alfons R.
-Author-email: alfonsrv@pm.me
+Author-email: alfonsrv@protonmail.com
 Maintainer: Alfons R.
-Maintainer-email: alfonsrv@pm.me
+Maintainer-email: alfonsrv@protonmail.com
 License: MIT
 Keywords: mail,email,parser
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 ### Multi-language email reply parsing for international environments 🌍
 
 Mail clients handle reply formatting differently, making reliable parsing difficult. Thank god we have 
 [standards](https://xkcd.com/927/).  This library splits *text-based* emails into separate replies based on common 
 headers produced by different, multilingual clients usually indicating separation.
 
 Replies can either present the whole mail message body, or strip headers, signatures and common disclaimers if required. 
-Currently supported languages are: English (`en`), German (`de`), French (`fr`), Italian (`it`) and Japanese (`ja`) – 
+Currently supported languages are: English (`en`), German (`de`), French (`fr`), Italian (`it`), Japanese (`ja`), Polish (`pl`) – 
 adding more languages is quite easy.
 
 This is an improved Python implementation of GitHub's Ruby-based [email_reply_parser](https://github.com/github/email_reply_parser/) 
 and an adaptation of Zapier's [email-reply-parser](https://github.com/zapier/email-reply-parser) which both split the 
 mails in fragments instead of distinct replies. They also only support English.
 
 
@@ -95,23 +95,24 @@
 
 *Or* get only the latest reply using:
 
 ```python
 latest_reply = EmailReplyParser(languages=languages).parse_reply(text=mail_body)
 ```
 
+
 ### Parser API
 
 ```
 EmailMessage.text:              Mail body
 EmailMessage.languages:         Languages to use for parsing headers
 EmailMessage.replies:           List of EmailReply; single parsed replies
 EmailMessage.include_english:   Always include English language for parsing
 EmailMessage.default_language:  Default language to use if language dictionary 
-                                doesn't include
+                                doesn't include any other language codes
 
 EmailMessage.HEADER_REGEX:      RegEx for identifying headers, separating mails
 EmailMessage.SIGNATURE_REGEX:   RegEx for identifying signatures
 EmailMessage.DISCLAIMERS_REGEX: RegEx for identifying disclaimers
 
 EmailMessage.read(): Parse EmailMessage.text to EmailReply which are then stored 
                      in EmailMessage.replies
```

### Comparing `mail-parser-reply-1.25/mailparser_reply/constants.py` & `mail_parser_reply-1.26/mailparser_reply/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#: Fallback language if no other language is specified
 from typing import Dict
 
+#: Fallback language if no other language is specified
 MAIL_LANGUAGE_DEFAULT = 'en'
 
 #: Matches text-mail quotation (usually starting with ">");
 #: resulting in "> Hello world"
 QUOTED_REGEX = r'(>+)'
 #: Regex to remove all leading quotations
 QUOTED_REMOVAL_REGEX = r'^(> *)'
@@ -45,20 +45,22 @@
             r'Mit freundlichen Gr\u00fc\u00DFen',
             r'Mit freundlichen Gr\u00fc\u00DFen / (?:Best|Kind) regards,',
             r'(?:(?:Beste(?:n)?|Liebe|Viele) )?(?:Gr(?:\u00fc|ue)(?:\u00DF|ss)(?:e)?|Gru\u00DF|Gruss)'
         ],
         'sent_from': 'Gesendet von',
     },
     'en': {
+        # Apple Mail-style header
         # ^(?!On[.\s]*On\s(.+?\s?.+?)\swrote:) – Negative lookahead, see:
         #    https://github.com/github/email_reply_parser/pull/31
         # <QUOTED_MATCH_INCLUDE> – allow matching this inside quoted levels
         # On\s(?:.+?\s?.+?)\swrote:) – match "On 01.01.2025, John Doe wrote:"
         #   See multiline_on.txt for example data
         'wrote_header': r'^(?!On[.\s]*On\s(.+?\s?.+?)\swrote:)(' + QUOTED_MATCH_INCLUDE + r'On\s(?:.+?\s?.+?)\s?wrote:)$',
+        # Outlook-style header
         # (?:(?:^|\n)[* ]*(?:From|Sent|To|Subject|Date|Cc):[ *]* – match From:/*From*:, ... headers
         # (?:\s{,2}).*){2,} – allow multi-line headers; some clients split the headers up into multiple lines.
         #       Also require at least two occurrences of the above pattern; e.g. From: ...\n Sent: ...
         # (?:\n.*){,1} – allow optional subject or other broken multi-line at the end
         'from_header': r'((?:(?:^|\n|\n' + QUOTED_MATCH_INCLUDE + r')[* ]*(?:From|Sent|To|Subject|Date|Cc):[ *]*(?:\s{,2}).*){2,}(?:\n.*){,1})',
         'disclaimers': [
             'CAUTION:',
@@ -106,13 +108,26 @@
         "from_header": r"((?:(?:^|\n|\n"
                        + QUOTED_MATCH_INCLUDE
                        + r")[* ]*(?:From|Sent|To|Subject|Date|Cc):[ *]*(?:\s{,2}).*){2,}(?:\n.*){,1})",
         "disclaimers": [],
         "signatures": [],
         "sent_from": "",
     },
+    "pl": {
+        'wrote_header': r'^(?!Dnia[.\s]*Dnia\s(.+?\s?.+?)\snadesłał:)(' + QUOTED_MATCH_INCLUDE + r'Dnia\s(?:.+?\s?.+?)\s?nadesłał:)$',
+        'from_header': r'((?:(?:^|\n|\n' + QUOTED_MATCH_INCLUDE + r')[* ]*(?:Od|Wysłano|Do|Temat|Data|DW):[ *]*(?:\s{,2}).*){2,}(?:\n.*){,1})',
+        "disclaimers": [
+            "Uwaga:"
+            ],
+        "signatures": [
+            "Z poważaniem",
+            "Z powazaniem",
+            "Pozdrawiam",
+            "W przypadku niejasności, proszę o kontakt."
+            ],
+        "sent_from": "Wysłano z"
+    },
     'david': {
         # Custom Software Headers – also kind of like a language, right?
         'from_header': r'((?:^ *Original Message processed by david.+?$\n{,7})(?:.*\n){,3}(?:(?:^|\n)[* ]*(?:Von|An|Cc)(?:\s{,2}).*){2,})'
-    }
+    },
 }
-
```

### Comparing `mail-parser-reply-1.25/mailparser_reply/parser.py` & `mail_parser_reply-1.26/mailparser_reply/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
     def parse_reply(self, text: str) -> Union[str, None]:
         """ Provides the latest reply portion of email.
         text - A string email body """
         return self.read(text).latest_reply
 
 
-
 @dataclass
 class EmailMessage:
     """ An email message represents a parsed email body. """
 
     #: Email message text body
     text: str
```

### Comparing `mail-parser-reply-1.25/setup.py` & `mail_parser_reply-1.26/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,17 +19,17 @@
     version=version.VERSION,
     description='📧 Email reply parser library for Python with multi-language support',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['mailparser_reply'],
     package_data={'mailparser_reply': ['../VERSION']},
     author='Alfons R.',
-    author_email='alfonsrv@pm.me',
+    author_email='alfonsrv@protonmail.com',
     maintainer="Alfons R.",
-    maintainer_email='alfonsrv@pm.me',
+    maintainer_email='alfonsrv@protonmail.com',
     url='https://github.com/alfonsrv/mail-parser-reply',
     license='MIT',
     test_suite='test',
     keywords=['mail', 'email', 'parser'],
     classifiers=[
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
```

### Comparing `mail-parser-reply-1.25/test/test_email_reply_parser.py` & `mail_parser_reply-1.26/test/test_email_reply_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,14 +124,36 @@
         mail = self.get_email('email_ja_1_2', parse=True, languages=['ja'])
         self.assertEqual(2, len(mail.replies))
         self.assertTrue("お世話になっております。織田です。" in mail.replies[0].body)
         self.assertTrue("それでは 11:00 にお待ちしております。" in mail.replies[0].body)
         self.assertTrue("かしこまりました" in mail.replies[1].body)
         self.assertTrue("明日の 11:00 でお願いいたします" in mail.replies[1].body)
 
+    def test_pl_simple_body(self):
+        mail = self.get_email('email_pl_1_1', parse=True, languages=['pl'])
+        self.assertEqual(1, len(mail.replies))
+        self.assertTrue("Czesc Anno" in mail.replies[0].body)
+        self.assertTrue("Pozdrawiam,\nJan" in mail.replies[0].signatures)
+        self.assertTrue("Pozdrawiam,\nJan" not in mail.replies[0].body)
+
+    def test_pl_simple_quoted_reply(self):
+        mail = self.get_email('email_pl_1_2', parse=True, languages=['pl'])
+        self.assertEqual(2, len(mail.replies))
+        self.assertTrue("Dnia 28 lutego 2023 14:00 Anna Nowak <anna.nowak@example.com>" in mail.replies[1].content)
+        self.assertTrue("Dnia 28 lutego 2023 14:00 Anna Nowak <anna.nowak@example.com>" not in mail.replies[1].body)
+        self.assertTrue("> Pozdrawiam," in mail.replies[1].content)
+        self.assertTrue("> Pozdrawiam," in mail.replies[1].signatures)
+        self.assertTrue("> Pozdrawiam," not in mail.replies[1].body)
+
+    def test_pl_simple_signature(self):
+        mail = self.get_email('email_pl_1_3', parse=True, languages=['pl'])
+        self.assertEqual(1, len(mail.replies))
+        self.assertTrue("Z powazaniem,\nJan" in mail.replies[0].signatures)
+        self.assertTrue("Z powazaniem,\nJan" not in mail.replies[0].body)
+
     def get_email(self, name: str, parse: bool = True, languages: list = None):
         """ Return EmailMessage instance or text content """
         with open(f'test/emails/{name}.txt') as f:
             text = f.read()
         return EmailReplyParser(
             languages=languages or [MAIL_LANGUAGE_DEFAULT]
         ).read(text) if parse else text
```

