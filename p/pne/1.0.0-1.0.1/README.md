# Comparing `tmp/pne-1.0.0.tar.gz` & `tmp/pne-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pne-1.0.0.tar", max compression
+gzip compressed data, was "pne-1.0.1.tar", max compression
```

## Comparing `pne-1.0.0.tar` & `pne-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11086 2024-05-18 19:19:54.758437 pne-1.0.0/LICENSE
--rw-r--r--   0        0        0     1533 2024-05-18 19:25:23.343148 pne-1.0.0/pne/__init__.py
--rw-r--r--   0        0        0     2526 2024-05-18 19:33:05.576752 pne-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1315 2024-05-18 19:29:53.988896 pne-1.0.0/README.md
--rw-r--r--   0        0        0     2131 1970-01-01 00:00:00.000000 pne-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10880 2024-05-25 11:03:14.033254 pne-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1281 2024-05-25 11:03:14.033254 pne-1.0.1/README.md
+-rw-r--r--   0        0        0     1499 2024-05-25 11:03:14.033254 pne-1.0.1/pne/__init__.py
+-rw-r--r--   0        0        0     2415 2024-05-25 11:03:14.033254 pne-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2131 1970-01-01 00:00:00.000000 pne-1.0.1/PKG-INFO
```

### Comparing `pne-1.0.0/LICENSE` & `pne-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,207 +1,207 @@
-Apache License
-Version 2.0, January 2004
-http://www.apache.org/licenses/
-
-TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-1. Definitions.
-
-    "License" shall mean the terms and conditions for use, reproduction, and
-    distribution as defined by Sections 1 through 9 of this document.
-
-    "Licensor" shall mean the copyright owner or entity authorized by the
-    copyright owner that is granting the License.
-
-    "Legal Entity" shall mean the union of the acting entity and all other
-    entities that control, are controlled by, or are under common control with
-    that entity. For the purposes of this definition, "control" means (i) the
-    power, direct or indirect, to cause the direction or management of such
-    entity, whether by contract or otherwise, or (ii) ownership of
-    fifty percent (50%) or more of the outstanding shares, or (iii) beneficial
-    ownership of such entity.
-
-    "You" (or "Your") shall mean an individual or Legal Entity exercising
-    permissions granted by this License.
-
-    "Source" form shall mean the preferred form for making modifications,
-    including but not limited to software source code, documentation source,
-    and configuration files.
-
-    "Object" form shall mean any form resulting from mechanical transformation
-    or translation of a Source form, including but not limited to compiled
-    object code, generated documentation, and conversions to
-    other media types.
-
-    "Work" shall mean the work of authorship, whether in Source or Object
-    form, made available under the License, as indicated by a copyright notice
-    that is included in or attached to the work (an example is provided in the
-    Appendix below).
-
-    "Derivative Works" shall mean any work, whether in Source or Object form,
-    that is based on (or derived from) the Work and for which the editorial
-    revisions, annotations, elaborations, or other modifications represent,
-    as a whole, an original work of authorship. For the purposes of this
-    License, Derivative Works shall not include works that remain separable
-    from, or merely link (or bind by name) to the interfaces of, the Work and
-    Derivative Works thereof.
-
-    "Contribution" shall mean any work of authorship, including the original
-    version of the Work and any modifications or additions to that Work or
-    Derivative Works thereof, that is intentionally submitted to Licensor for
-    inclusion in the Work by the copyright owner or by an individual or
-    Legal Entity authorized to submit on behalf of the copyright owner.
-    For the purposes of this definition, "submitted" means any form of
-    electronic, verbal, or written communication sent to the Licensor or its
-    representatives, including but not limited to communication on electronic
-    mailing lists, source code control systems, and issue tracking systems
-    that are managed by, or on behalf of, the Licensor for the purpose of
-    discussing and improving the Work, but excluding communication that is
-    conspicuously marked or otherwise designated in writing by the copyright
-    owner as "Not a Contribution."
-
-    "Contributor" shall mean Licensor and any individual or Legal Entity on
-    behalf of whom a Contribution has been received by Licensor and
-    subsequently incorporated within the Work.
-
-2. Grant of Copyright License.
-
-    Subject to the terms and conditions of this License, each Contributor
-    hereby grants to You a perpetual, worldwide, non-exclusive, no-charge,
-    royalty-free, irrevocable copyright license to reproduce, prepare
-    Derivative Works of, publicly display, publicly perform, sublicense,
-    and distribute the Work and such Derivative Works in
-    Source or Object form.
-
-3. Grant of Patent License.
-
-    Subject to the terms and conditions of this License, each Contributor
-    hereby grants to You a perpetual, worldwide, non-exclusive, no-charge,
-    royalty-free, irrevocable (except as stated in this section) patent
-    license to make, have made, use, offer to sell, sell, import, and
-    otherwise transfer the Work, where such license applies only to those
-    patent claims licensable by such Contributor that are necessarily
-    infringed by their Contribution(s) alone or by combination of their
-    Contribution(s) with the Work to which such Contribution(s) was submitted.
-    If You institute patent litigation against any entity (including a
-    cross-claim or counterclaim in a lawsuit) alleging that the Work or a
-    Contribution incorporated within the Work constitutes direct or
-    contributory patent infringement, then any patent licenses granted to
-    You under this License for that Work shall terminate as of the date such
-    litigation is filed.
-
-4. Redistribution.
-
-    You may reproduce and distribute copies of the Work or Derivative Works
-    thereof in any medium, with or without modifications, and in Source or
-    Object form, provided that You meet the following conditions:
-
-    1. You must give any other recipients of the Work or Derivative Works a
-    copy of this License; and
-
-    2. You must cause any modified files to carry prominent notices stating
-    that You changed the files; and
-
-    3. You must retain, in the Source form of any Derivative Works that You
-    distribute, all copyright, patent, trademark, and attribution notices from
-    the Source form of the Work, excluding those notices that do not pertain
-    to any part of the Derivative Works; and
-
-    4. If the Work includes a "NOTICE" text file as part of its distribution,
-    then any Derivative Works that You distribute must include a readable copy
-    of the attribution notices contained within such NOTICE file, excluding
-    those notices that do not pertain to any part of the Derivative Works,
-    in at least one of the following places: within a NOTICE text file
-    distributed as part of the Derivative Works; within the Source form or
-    documentation, if provided along with the Derivative Works; or, within a
-    display generated by the Derivative Works, if and wherever such
-    third-party notices normally appear. The contents of the NOTICE file are
-    for informational purposes only and do not modify the License.
-    You may add Your own attribution notices within Derivative Works that You
-    distribute, alongside or as an addendum to the NOTICE text from the Work,
-    provided that such additional attribution notices cannot be construed
-    as modifying the License.
-
-    You may add Your own copyright statement to Your modifications and may
-    provide additional or different license terms and conditions for use,
-    reproduction, or distribution of Your modifications, or for any such
-    Derivative Works as a whole, provided Your use, reproduction, and
-    distribution of the Work otherwise complies with the conditions
-    stated in this License.
-
-5. Submission of Contributions.
-
-    Unless You explicitly state otherwise, any Contribution intentionally
-    submitted for inclusion in the Work by You to the Licensor shall be under
-    the terms and conditions of this License, without any additional
-    terms or conditions. Notwithstanding the above, nothing herein shall
-    supersede or modify the terms of any separate license agreement you may
-    have executed with Licensor regarding such Contributions.
-
-6. Trademarks.
-
-    This License does not grant permission to use the trade names, trademarks,
-    service marks, or product names of the Licensor, except as required for
-    reasonable and customary use in describing the origin of the Work and
-    reproducing the content of the NOTICE file.
-
-7. Disclaimer of Warranty.
-
-    Unless required by applicable law or agreed to in writing, Licensor
-    provides the Work (and each Contributor provides its Contributions)
-    on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
-    either express or implied, including, without limitation, any warranties
-    or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS
-    FOR A PARTICULAR PURPOSE. You are solely responsible for determining the
-    appropriateness of using or redistributing the Work and assume any risks
-    associated with Your exercise of permissions under this License.
-
-8. Limitation of Liability.
-
-    In no event and under no legal theory, whether in tort
-    (including negligence), contract, or otherwise, unless required by
-    applicable law (such as deliberate and grossly negligent acts) or agreed
-    to in writing, shall any Contributor be liable to You for damages,
-    including any direct, indirect, special, incidental, or consequential
-    damages of any character arising as a result of this License or out of
-    the use or inability to use the Work (including but not limited to damages
-    for loss of goodwill, work stoppage, computer failure or malfunction,
-    or any and all other commercial damages or losses), even if such
-    Contributor has been advised of the possibility of such damages.
-
-9. Accepting Warranty or Additional Liability.
-
-    While redistributing the Work or Derivative Works thereof, You may choose
-    to offer, and charge a fee for, acceptance of support, warranty,
-    indemnity, or other liability obligations and/or rights consistent with
-    this License. However, in accepting such obligations, You may act only
-    on Your own behalf and on Your sole responsibility, not on behalf of any
-    other Contributor, and only if You agree to indemnify, defend, and hold
-    each Contributor harmless for any liability incurred by, or claims
-    asserted against, such Contributor by reason of your accepting any such
-    warranty or additional liability.
-
-END OF TERMS AND CONDITIONS
-
-APPENDIX: How to apply the Apache License to your work
-
-    To apply the Apache License to your work, attach the following boilerplate
-    notice, with the fields enclosed by brackets "[]" replaced with your own
-    identifying information. (Don't include the brackets!) The text should be
-    enclosed in the appropriate comment syntax for the file format. We also
-    recommend that a file or class name and description of purpose be included
-    on the same "printed page" as the copyright notice for easier
-    identification within third-party archives.
-
-        Copyright 2024 pne
-
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
-        or implied. See the License for the specific language governing
+Apache License
+Version 2.0, January 2004
+http://www.apache.org/licenses/
+
+TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+1. Definitions.
+
+    "License" shall mean the terms and conditions for use, reproduction, and
+    distribution as defined by Sections 1 through 9 of this document.
+
+    "Licensor" shall mean the copyright owner or entity authorized by the
+    copyright owner that is granting the License.
+
+    "Legal Entity" shall mean the union of the acting entity and all other
+    entities that control, are controlled by, or are under common control with
+    that entity. For the purposes of this definition, "control" means (i) the
+    power, direct or indirect, to cause the direction or management of such
+    entity, whether by contract or otherwise, or (ii) ownership of
+    fifty percent (50%) or more of the outstanding shares, or (iii) beneficial
+    ownership of such entity.
+
+    "You" (or "Your") shall mean an individual or Legal Entity exercising
+    permissions granted by this License.
+
+    "Source" form shall mean the preferred form for making modifications,
+    including but not limited to software source code, documentation source,
+    and configuration files.
+
+    "Object" form shall mean any form resulting from mechanical transformation
+    or translation of a Source form, including but not limited to compiled
+    object code, generated documentation, and conversions to
+    other media types.
+
+    "Work" shall mean the work of authorship, whether in Source or Object
+    form, made available under the License, as indicated by a copyright notice
+    that is included in or attached to the work (an example is provided in the
+    Appendix below).
+
+    "Derivative Works" shall mean any work, whether in Source or Object form,
+    that is based on (or derived from) the Work and for which the editorial
+    revisions, annotations, elaborations, or other modifications represent,
+    as a whole, an original work of authorship. For the purposes of this
+    License, Derivative Works shall not include works that remain separable
+    from, or merely link (or bind by name) to the interfaces of, the Work and
+    Derivative Works thereof.
+
+    "Contribution" shall mean any work of authorship, including the original
+    version of the Work and any modifications or additions to that Work or
+    Derivative Works thereof, that is intentionally submitted to Licensor for
+    inclusion in the Work by the copyright owner or by an individual or
+    Legal Entity authorized to submit on behalf of the copyright owner.
+    For the purposes of this definition, "submitted" means any form of
+    electronic, verbal, or written communication sent to the Licensor or its
+    representatives, including but not limited to communication on electronic
+    mailing lists, source code control systems, and issue tracking systems
+    that are managed by, or on behalf of, the Licensor for the purpose of
+    discussing and improving the Work, but excluding communication that is
+    conspicuously marked or otherwise designated in writing by the copyright
+    owner as "Not a Contribution."
+
+    "Contributor" shall mean Licensor and any individual or Legal Entity on
+    behalf of whom a Contribution has been received by Licensor and
+    subsequently incorporated within the Work.
+
+2. Grant of Copyright License.
+
+    Subject to the terms and conditions of this License, each Contributor
+    hereby grants to You a perpetual, worldwide, non-exclusive, no-charge,
+    royalty-free, irrevocable copyright license to reproduce, prepare
+    Derivative Works of, publicly display, publicly perform, sublicense,
+    and distribute the Work and such Derivative Works in
+    Source or Object form.
+
+3. Grant of Patent License.
+
+    Subject to the terms and conditions of this License, each Contributor
+    hereby grants to You a perpetual, worldwide, non-exclusive, no-charge,
+    royalty-free, irrevocable (except as stated in this section) patent
+    license to make, have made, use, offer to sell, sell, import, and
+    otherwise transfer the Work, where such license applies only to those
+    patent claims licensable by such Contributor that are necessarily
+    infringed by their Contribution(s) alone or by combination of their
+    Contribution(s) with the Work to which such Contribution(s) was submitted.
+    If You institute patent litigation against any entity (including a
+    cross-claim or counterclaim in a lawsuit) alleging that the Work or a
+    Contribution incorporated within the Work constitutes direct or
+    contributory patent infringement, then any patent licenses granted to
+    You under this License for that Work shall terminate as of the date such
+    litigation is filed.
+
+4. Redistribution.
+
+    You may reproduce and distribute copies of the Work or Derivative Works
+    thereof in any medium, with or without modifications, and in Source or
+    Object form, provided that You meet the following conditions:
+
+    1. You must give any other recipients of the Work or Derivative Works a
+    copy of this License; and
+
+    2. You must cause any modified files to carry prominent notices stating
+    that You changed the files; and
+
+    3. You must retain, in the Source form of any Derivative Works that You
+    distribute, all copyright, patent, trademark, and attribution notices from
+    the Source form of the Work, excluding those notices that do not pertain
+    to any part of the Derivative Works; and
+
+    4. If the Work includes a "NOTICE" text file as part of its distribution,
+    then any Derivative Works that You distribute must include a readable copy
+    of the attribution notices contained within such NOTICE file, excluding
+    those notices that do not pertain to any part of the Derivative Works,
+    in at least one of the following places: within a NOTICE text file
+    distributed as part of the Derivative Works; within the Source form or
+    documentation, if provided along with the Derivative Works; or, within a
+    display generated by the Derivative Works, if and wherever such
+    third-party notices normally appear. The contents of the NOTICE file are
+    for informational purposes only and do not modify the License.
+    You may add Your own attribution notices within Derivative Works that You
+    distribute, alongside or as an addendum to the NOTICE text from the Work,
+    provided that such additional attribution notices cannot be construed
+    as modifying the License.
+
+    You may add Your own copyright statement to Your modifications and may
+    provide additional or different license terms and conditions for use,
+    reproduction, or distribution of Your modifications, or for any such
+    Derivative Works as a whole, provided Your use, reproduction, and
+    distribution of the Work otherwise complies with the conditions
+    stated in this License.
+
+5. Submission of Contributions.
+
+    Unless You explicitly state otherwise, any Contribution intentionally
+    submitted for inclusion in the Work by You to the Licensor shall be under
+    the terms and conditions of this License, without any additional
+    terms or conditions. Notwithstanding the above, nothing herein shall
+    supersede or modify the terms of any separate license agreement you may
+    have executed with Licensor regarding such Contributions.
+
+6. Trademarks.
+
+    This License does not grant permission to use the trade names, trademarks,
+    service marks, or product names of the Licensor, except as required for
+    reasonable and customary use in describing the origin of the Work and
+    reproducing the content of the NOTICE file.
+
+7. Disclaimer of Warranty.
+
+    Unless required by applicable law or agreed to in writing, Licensor
+    provides the Work (and each Contributor provides its Contributions)
+    on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
+    either express or implied, including, without limitation, any warranties
+    or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS
+    FOR A PARTICULAR PURPOSE. You are solely responsible for determining the
+    appropriateness of using or redistributing the Work and assume any risks
+    associated with Your exercise of permissions under this License.
+
+8. Limitation of Liability.
+
+    In no event and under no legal theory, whether in tort
+    (including negligence), contract, or otherwise, unless required by
+    applicable law (such as deliberate and grossly negligent acts) or agreed
+    to in writing, shall any Contributor be liable to You for damages,
+    including any direct, indirect, special, incidental, or consequential
+    damages of any character arising as a result of this License or out of
+    the use or inability to use the Work (including but not limited to damages
+    for loss of goodwill, work stoppage, computer failure or malfunction,
+    or any and all other commercial damages or losses), even if such
+    Contributor has been advised of the possibility of such damages.
+
+9. Accepting Warranty or Additional Liability.
+
+    While redistributing the Work or Derivative Works thereof, You may choose
+    to offer, and charge a fee for, acceptance of support, warranty,
+    indemnity, or other liability obligations and/or rights consistent with
+    this License. However, in accepting such obligations, You may act only
+    on Your own behalf and on Your sole responsibility, not on behalf of any
+    other Contributor, and only if You agree to indemnify, defend, and hold
+    each Contributor harmless for any liability incurred by, or claims
+    asserted against, such Contributor by reason of your accepting any such
+    warranty or additional liability.
+
+END OF TERMS AND CONDITIONS
+
+APPENDIX: How to apply the Apache License to your work
+
+    To apply the Apache License to your work, attach the following boilerplate
+    notice, with the fields enclosed by brackets "[]" replaced with your own
+    identifying information. (Don't include the brackets!) The text should be
+    enclosed in the appropriate comment syntax for the file format. We also
+    recommend that a file or class name and description of purpose be included
+    on the same "printed page" as the copyright notice for easier
+    identification within third-party archives.
+
+        Copyright 2024 pne
+
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
+        or implied. See the License for the specific language governing
         permissions and limitations under the License.
```

### Comparing `pne-1.0.0/pne/__init__.py` & `pne-1.0.1/pne/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,63 @@
-import warnings
-
-from promptulate.agents.assistant_agent.agent import AssistantAgent
-from promptulate.agents.base import BaseAgent
-from promptulate.agents.planner.planner import Planner
-from promptulate.agents.tool_agent.agent import ToolAgent
-from promptulate.agents.web_agent.agent import WebAgent
-from promptulate.chat import AIChat, chat
-from promptulate.llms.base import BaseLLM
-from promptulate.llms.factory import LLMFactory
-from promptulate.llms.openai.openai import ChatOpenAI
-from promptulate.output_formatter import OutputFormatter
-from promptulate.schema import (
-    AssistantMessage,
-    BaseMessage,
-    MessageSet,
-    SystemMessage,
-    UserMessage,
-)
-from promptulate.tools.base import BaseTool, Tool, define_tool
-from promptulate.utils.logger import enable_log
-from promptulate.utils.string_template import StringTemplate
-
-_util_fields = [
-    "enable_log",
-    "OutputFormatter",
-    "StringTemplate",
-]
-
-_schema_fields = [
-    "AssistantMessage",
-    "SystemMessage",
-    "UserMessage",
-    "BaseMessage",
-    "MessageSet",
-]
-
-_llm_fields = ["chat", "AIChat", "BaseLLM", "ChatOpenAI", "LLMFactory"]
-
-_tool_fields = [
-    "Tool",
-    "define_tool",
-    "BaseTool",
-]
-
-_agent_fields = [
-    "BaseAgent",
-    "WebAgent",
-    "ToolAgent",
-    "AssistantAgent",
-    "Planner",
-]
-
-__all__ = [
-    *_util_fields,
-    *_schema_fields,
-    *_llm_fields,
-    *_tool_fields,
-    *_agent_fields,
-]
-
-warnings.filterwarnings("always", category=DeprecationWarning)
+import warnings
+
+from promptulate.agents.assistant_agent.agent import AssistantAgent
+from promptulate.agents.base import BaseAgent
+from promptulate.agents.planner.planner import Planner
+from promptulate.agents.tool_agent.agent import ToolAgent
+from promptulate.agents.web_agent.agent import WebAgent
+from promptulate.chat import AIChat, chat
+from promptulate.llms.base import BaseLLM
+from promptulate.llms.factory import LLMFactory
+from promptulate.llms.openai.openai import ChatOpenAI
+from promptulate.output_formatter import OutputFormatter
+from promptulate.schema import (
+    AssistantMessage,
+    BaseMessage,
+    MessageSet,
+    SystemMessage,
+    UserMessage,
+)
+from promptulate.tools.base import BaseTool, Tool, ToolTypes, define_tool
+from promptulate.utils.logger import enable_log
+from promptulate.utils.string_template import StringTemplate
+
+_util_fields = [
+    "enable_log",
+    "OutputFormatter",
+    "StringTemplate",
+]
+
+_schema_fields = [
+    "AssistantMessage",
+    "SystemMessage",
+    "UserMessage",
+    "BaseMessage",
+    "MessageSet",
+]
+
+_llm_fields = ["chat", "AIChat", "BaseLLM", "ChatOpenAI", "LLMFactory"]
+
+_tool_fields = [
+    "Tool",
+    "define_tool",
+    "BaseTool",
+    "ToolTypes",
+]
+
+_agent_fields = [
+    "BaseAgent",
+    "WebAgent",
+    "ToolAgent",
+    "AssistantAgent",
+    "Planner",
+]
+
+__all__ = [
+    *_util_fields,
+    *_schema_fields,
+    *_llm_fields,
+    *_tool_fields,
+    *_agent_fields,
+]
+
+warnings.filterwarnings("always", category=DeprecationWarning)
```

### Comparing `pne-1.0.0/README.md` & `pne-1.0.1/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# pne
-
-<div align="center">
-
-
-[![Python Version](https://img.shields.io/pypi/pyversions/pne.svg)](https://pypi.org/project/pne/)
-[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/Undertone0809/pne/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
-[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/Undertone0809/pne/releases)
-[![License](https://img.shields.io/github/license/Undertone0809/pne)](https://github.com/Undertone0809/pne/blob/main/LICENSE)
-
-
-🚀 Simplified promptulate call. Now you can use `import pne` to call [promptulate](https://github.com/Undertone0809/promptulate).
-
-</div>
-
-## Quick start
-
-Conda package manager is recommended. Create a conda environment.
-
-```bash
-pip install pne
-```
-
-Then you can anything function like promptulate:
-
-```python
-import pne
-
-pne.chat(messages="Hello, world!", model="gpt-4-turbo")
-```
-
-## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/3PG-%F0%9F%9A%80-brightgreen)](https://github.com/Undertone0809/python-package-template)
-
-This project was generated with [3PG](https://github.com/Undertone0809/3PG)
+# pne
+
+<div align="center">
+
+
+[![Python Version](https://img.shields.io/pypi/pyversions/pne.svg)](https://pypi.org/project/pne/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/Undertone0809/pne/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/Undertone0809/pne/releases)
+[![License](https://img.shields.io/github/license/Undertone0809/pne)](https://github.com/Undertone0809/pne/blob/main/LICENSE)
+
+
+🚀 Simplified promptulate call. Now you can use `import pne` to call [promptulate](https://github.com/Undertone0809/promptulate).
+
+</div>
+
+## Quick start
+
+Conda package manager is recommended. Create a conda environment.
+
+```bash
+pip install pne
+```
+
+Then you can anything function like promptulate:
+
+```python
+import pne
+
+pne.chat(messages="Hello, world!", model="gpt-4-turbo")
+```
+
+## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/3PG-%F0%9F%9A%80-brightgreen)](https://github.com/Undertone0809/python-package-template)
+
+This project was generated with [3PG](https://github.com/Undertone0809/3PG)
```

### Comparing `pne-1.0.0/PKG-INFO` & `pne-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pne
-Version: 1.0.0
+Version: 1.0.1
 Summary: 🚀 Simplified promptulate call. Now you can use `import pne` to call promptulate.
 Home-page: https://github.com/Undertone0809/pne
 License: Apache Software License 2.0
 Keywords: promptulate,pne,prompt,agent,openai,chatgpt,gpt,llm,openai,langchain,litellm
 Author: Undertone0809
 Author-email: zeeland4work@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: promptulate (>=1.16.5,<2.0.0)
+Requires-Dist: promptulate (>=1.16.6,<2.0.0)
 Project-URL: Repository, https://github.com/Undertone0809/pne
 Description-Content-Type: text/markdown
 
 # pne
 
 <div align="center">
```

