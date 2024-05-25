# Comparing `tmp/mail_devel-0.8.2-py3-none-any.whl.zip` & `tmp/mail_devel-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 20733 bytes, number of entries: 18
--rw-r--r--  2.0 unx       48 b- defN 24-Jan-11 19:43 mail_devel/__init__.py
+Zip file size: 21255 bytes, number of entries: 18
+-rw-r--r--  2.0 unx       48 b- defN 24-Mar-28 21:16 mail_devel/__init__.py
 -rw-r--r--  2.0 unx      914 b- defN 23-Nov-25 14:41 mail_devel/__main__.py
 -rw-r--r--  2.0 unx     1956 b- defN 23-Nov-25 14:11 mail_devel/auth.py
--rw-r--r--  2.0 unx    13877 b- defN 23-Dec-18 17:12 mail_devel/http.py
--rw-r--r--  2.0 unx     3205 b- defN 23-Nov-25 14:11 mail_devel/mailbox.py
+-rw-r--r--  2.0 unx    14797 b- defN 24-Mar-28 21:09 mail_devel/http.py
+-rw-r--r--  2.0 unx     4379 b- defN 24-Mar-28 20:08 mail_devel/mailbox.py
 -rw-r--r--  2.0 unx    10918 b- defN 23-Nov-30 18:08 mail_devel/service.py
--rw-r--r--  2.0 unx     1312 b- defN 23-Nov-25 14:11 mail_devel/smtp.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-Mar-28 20:09 mail_devel/smtp.py
 -rw-r--r--  2.0 unx     3133 b- defN 23-Nov-30 18:04 mail_devel/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-18 17:37 mail_devel/resources/__init__.py
--rw-r--r--  2.0 unx     4894 b- defN 23-Dec-14 21:08 mail_devel/resources/index.html
--rw-r--r--  2.0 unx     6160 b- defN 24-Jan-11 20:03 mail_devel/resources/main.css
--rw-r--r--  2.0 unx    15485 b- defN 24-Jan-11 21:56 mail_devel/resources/main.js
--rw-r--r--  2.0 unx     1085 b- defN 24-Jan-11 21:57 mail_devel-0.8.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1519 b- defN 24-Jan-11 21:57 mail_devel-0.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-11 21:57 mail_devel-0.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 24-Jan-11 21:57 mail_devel-0.8.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Jan-11 21:57 mail_devel-0.8.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1459 b- defN 24-Jan-11 21:57 mail_devel-0.8.2.dist-info/RECORD
-18 files, 66124 bytes uncompressed, 18351 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx     4925 b- defN 24-Mar-04 18:42 mail_devel/resources/index.html
+-rw-r--r--  2.0 unx     6350 b- defN 24-Mar-04 18:45 mail_devel/resources/main.css
+-rw-r--r--  2.0 unx    16175 b- defN 24-Mar-28 20:38 mail_devel/resources/main.js
+-rw-r--r--  2.0 unx     1085 b- defN 24-Mar-28 21:16 mail_devel-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1519 b- defN 24-Mar-28 21:16 mail_devel-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-28 21:16 mail_devel-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 24-Mar-28 21:16 mail_devel-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Mar-28 21:16 mail_devel-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1459 b- defN 24-Mar-28 21:16 mail_devel-0.9.0.dist-info/RECORD
+18 files, 69119 bytes uncompressed, 18873 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: mail_devel/resources/main.css
 Comment: 
 
 Filename: mail_devel/resources/main.js
 Comment: 
 
-Filename: mail_devel-0.8.2.dist-info/LICENSE
+Filename: mail_devel-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: mail_devel-0.8.2.dist-info/METADATA
+Filename: mail_devel-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: mail_devel-0.8.2.dist-info/WHEEL
+Filename: mail_devel-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: mail_devel-0.8.2.dist-info/entry_points.txt
+Filename: mail_devel-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mail_devel-0.8.2.dist-info/top_level.txt
+Filename: mail_devel-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mail_devel-0.8.2.dist-info/RECORD
+Filename: mail_devel-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mail_devel/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .service import Service
 
-VERSION = "0.8.2"
+VERSION = "0.9.0"
```

## mail_devel/http.py

```diff
@@ -92,28 +92,38 @@
             [
                 web.get("/", self._page_index),
                 web.get("/config", self._api_config),
                 web.get(r"/{static:.*\.(css|js)}", self._page_static),
                 web.post(r"/api", self._api_post),
                 web.post(r"/api/upload", self._api_upload),
                 web.get(r"/api", self._api_index),
-                web.get(r"/api/{user}", self._api_user),
-                web.get(r"/api/{user}/{mailbox}", self._api_mailbox),
-                web.get(r"/api/{user}/{mailbox}/{uid:\d+}", self._api_message),
-                web.get(r"/api/{user}/{mailbox}/{uid:\d+}/reply", self._api_reply),
+                web.get(r"/api/{account:\d+}", self._api_account),
+                web.get(r"/api/{account:\d+}/{mailbox:\d+}", self._api_mailbox),
                 web.get(
-                    r"/api/{user}/{mailbox}/{uid:\d+}/attachment/{attachment}",
+                    r"/api/{account:\d+}/{mailbox:\d+}/{uid:\d+}",
+                    self._api_message,
+                ),
+                web.get(
+                    r"/api/{account:\d+}/{mailbox:\d+}/{uid:\d+}/reply",
+                    self._api_reply,
+                ),
+                web.get(
+                    r"/api/{account:\d+}/{mailbox:\d+}/{uid:\d+}/attachment/{attachment}",
                     self._api_attachment,
                 ),
-                web.get(r"/api/{user}/{mailbox}/{uid:\d+}/flags", self._api_flag),
+                web.get(
+                    r"/api/{account:\d+}/{mailbox:\d+}/{uid:\d+}/flags", self._api_flag
+                ),
                 web.put(
-                    r"/api/{user}/{mailbox}/{uid:\d+}/flags/{flag}", self._api_flag
+                    r"/api/{account:\d+}/{mailbox:\d+}/{uid:\d+}/flags/{flag}",
+                    self._api_flag,
                 ),
                 web.delete(
-                    r"/api/{user}/{mailbox}/{uid:\d+}/flags/{flag}", self._api_flag
+                    r"/api/{account:\d+}/{mailbox:\d+}/{uid:\d+}/flags/{flag}",
+                    self._api_flag,
                 ),
             ]
         )
 
         return await run_app(
             self.api,
             host=self.host or None,
@@ -187,26 +197,30 @@
             {
                 "multi_user": self.multi_user,
                 "flagged_seen": self.flagged_seen,
             }
         )
 
     async def _api_index(self, request: Request) -> Response:  # pylint: disable=W0613
-        mailboxes = await self.mailboxes.list()
-        return web.json_response(mailboxes)
+        accounts = await self.mailboxes.list()
+        return web.json_response(
+            {self.mailboxes.id_of_user(user): user for user in accounts}
+        )
 
-    async def _api_user(self, request: Request) -> Response:  # pylint: disable=W0613
+    async def _api_account(self, request: Request) -> Response:  # pylint: disable=W0613
         try:
-            user = request.match_info["user"]
-            mailbox = self.mailboxes[user]
+            account_id = int(request.match_info["account"])
+            account = await self.mailboxes.get_by_id(account_id)
         except KeyError as e:  # pragma: no cover
             raise web.HTTPNotFound() from e
 
-        mailboxes = await mailbox.list_mailboxes()
-        return web.json_response([e.name for e in mailboxes.list()])
+        mailboxes = await account.list_mailboxes()
+        return web.json_response(
+            {account.id_of_mailbox(e.name): e.name for e in mailboxes.list()}
+        )
 
     async def _api_upload(self, request: Request) -> Response:  # pylint: disable=W0613
         data = await request.json()
         if not isinstance(data, list):
             raise web.HTTPBadRequest()
 
         compat_strict = policy.compat32.clone(raise_on_defect=True)
@@ -252,47 +266,50 @@
             message,
             flags=frozenset({Flag(b"\\Seen")} if self.flagged_seen else []),
         )
         return web.json_response({"status": "ok"})
 
     async def _api_mailbox(self, request: Request) -> Response:
         try:
-            user = request.match_info["user"]
-            name = request.match_info["mailbox"]
-            mailbox = await self.mailboxes[user].get_mailbox(name)
+            account_id = int(request.match_info["account"])
+            account = self.mailboxes.user_mapping[account_id]
+            mailbox_id = int(request.match_info["mailbox"])
+            mailbox = await self.mailboxes[account].get_mailbox_by_id(mailbox_id)
         except KeyError as e:  # pragma: no cover
             raise web.HTTPNotFound() from e
 
         result = []
         async for msg in mailbox.messages():
             result.append(await self._convert_message(msg))
         result.sort(key=lambda x: x["date"], reverse=True)
         return web.json_response(result)
 
     async def _api_message(self, request: Request) -> Response:
         try:
-            user = request.match_info["user"]
-            name = request.match_info["mailbox"]
+            account_id = int(request.match_info["account"])
+            account = self.mailboxes.user_mapping[account_id]
+            mailbox_id = int(request.match_info["mailbox"])
             uid = int(request.match_info["uid"])
-            mailbox = await self.mailboxes[user].get_mailbox(name)
+            mailbox = await self.mailboxes[account].get_mailbox_by_id(mailbox_id)
         except (IndexError, KeyError) as e:  # pragma: no cover
             raise web.HTTPNotFound() from e
 
         async for msg in mailbox.messages():
             if msg.uid == uid:
                 return web.json_response(await self._convert_message(msg, True))
 
         raise web.HTTPNotFound()
 
     async def _api_reply(self, request: Request) -> Response:
         try:
-            user = request.match_info["user"]
-            name = request.match_info["mailbox"]
+            account_id = int(request.match_info["account"])
+            mailbox_id = int(request.match_info["mailbox"])
             uid = int(request.match_info["uid"])
-            mailbox = await self.mailboxes[user].get_mailbox(name)
+            account = await self.mailboxes.get_by_id(account_id)
+            mailbox = await account.get_mailbox_by_id(mailbox_id)
         except (IndexError, KeyError) as e:  # pragma: no cover
             raise web.HTTPNotFound() from e
 
         async for msg in mailbox.messages():
             if msg.uid == uid:
                 message = await self._convert_message(msg, True)
                 headers = message["header"]
@@ -310,19 +327,20 @@
                         headers.pop(key, None)
                 return web.json_response(message)
 
         raise web.HTTPNotFound()
 
     async def _api_attachment(self, request: Request) -> Response:
         try:
-            user = request.match_info["user"]
-            name = request.match_info["mailbox"]
+            account_id = int(request.match_info["account"])
+            mailbox_id = int(request.match_info["mailbox"])
             uid = int(request.match_info["uid"])
             attachment = request.match_info["attachment"]
-            mailbox = await self.mailboxes[user].get_mailbox(name)
+            account = await self.mailboxes.get_by_id(account_id)
+            mailbox = await account.get_mailbox_by_id(mailbox_id)
         except (IndexError, KeyError) as e:  # pragma: no cover
             raise web.HTTPNotFound() from e
 
         message = None
         async for msg in mailbox.messages():
             if msg.uid == uid:
                 content = await self._message_content(msg)
@@ -346,17 +364,18 @@
                     },
                 )
 
         raise web.HTTPNotFound()
 
     async def _api_flag(self, request: Request) -> Response:
         try:
-            user = request.match_info["user"]
-            name = request.match_info["mailbox"]
-            mailbox = await self.mailboxes[user].get_mailbox(name)
+            account_id = int(request.match_info["account"])
+            mailbox_id = int(request.match_info["mailbox"])
+            account = await self.mailboxes.get_by_id(account_id)
+            mailbox = await account.get_mailbox_by_id(mailbox_id)
             uid = int(request.match_info["uid"])
 
             if request.method in ("DELETE", "PUT"):
                 flags = [Flag(b"\\" + request.match_info["flag"].title().encode())]
             else:
                 flags = []
         except (IndexError, KeyError) as e:  # pragma: no cover
```

## mail_devel/mailbox.py

```diff
@@ -10,50 +10,84 @@
 
 _logger = logging.getLogger(__name__)
 
 
 class TestMailboxSet(MailboxSet):
     """This MailboxSet creates the mailboxes automatically"""
 
+    def __init__(self):
+        super().__init__()
+        self.mailbox_mapping: dict[int, str] = {}
+
+    def id_of_mailbox(self, name: str) -> int:
+        for mailbox_id, mailbox_name in self.mailbox_mapping.items():
+            if mailbox_name == name:
+                return mailbox_id
+
+        new_id = len(self.mailbox_mapping) + 1
+        self.mailbox_mapping[new_id] = name
+        return new_id
+
+    async def get_mailbox_by_id(self, mailbox_id: int) -> MailboxData:
+        mailbox_name = self.mailbox_mapping[mailbox_id]
+        return await self.get_mailbox(mailbox_name)
+
     async def get_mailbox(self, name: str) -> MailboxData:
         if name not in self._set:
             await self.add_mailbox(name)
         return await super().get_mailbox(name)
 
 
 class TestMailboxDict:
     """Class to handle all mailbox accounts"""
 
     def __init__(
         self, config: IMAPConfig, filter_set: FilterSet, multi_user: bool = False
     ):
-        self.config = config
-        self.filter_set = filter_set
-        self.multi_user = multi_user
+        self.config: IMAPConfig = config
+        self.filter_set: FilterSet = filter_set
+        self.multi_user: bool = multi_user
+        self.user_mapping: dict[int, str] = {}
 
     def __contains__(self, user: str) -> bool:
         return not self.multi_user or user in self.config.set_cache
 
     def __getitem__(self, user: str) -> TestMailboxSet:
         return self.config.set_cache[user][0]
 
+    def id_of_user(self, name: str) -> int:
+        for uid, user_name in self.user_mapping.items():
+            if user_name == name:
+                return uid
+
+        new_id = len(self.user_mapping) + 1
+        self.user_mapping[new_id] = name
+        return new_id
+
     async def inbox_stats(self) -> dict[str, int]:
         stats = {}
         for user, (mset, _fset) in self.config.set_cache.items():
             mbox = await mset.get_mailbox("INBOX")
             stats[user] = len([msg async for msg in mbox.messages()])
         return stats
 
     async def list(self):
         """List the available mailbox accounts"""
         if not self.multi_user and not self.config.set_cache:
             await self.get(self.config.demo_user)
 
         return list(self.config.set_cache)
 
+    async def get_by_id(self, user_id: int) -> TestMailboxSet:
+        if not self.multi_user:
+            return await self.get(self.config.demo_user)
+
+        user_name = self.user_mapping[user_id]
+        return await self.get(user_name)
+
     async def get(self, user: str) -> TestMailboxSet:
         """Get the mailbox for the user or the main mailbox if single user mode"""
         if not self.multi_user:
             user = self.config.demo_user
 
         if user not in self.config.set_cache:
             mbox = TestMailboxSet()
```

## mail_devel/smtp.py

```diff
@@ -15,20 +15,19 @@
         self,
         mailboxes: TestMailboxDict,
         flagged_seen: bool = False,
         message_class: Type[Message] | None = None,
         multi_user: bool = False,
     ):
         super().__init__(message_class)
-        self.mailboxes = mailboxes
-        self.flagged_seen = flagged_seen
-        self.multi_user = multi_user
+        self.mailboxes: TestMailboxDict = mailboxes
+        self.flagged_seen: bool = flagged_seen
+        self.multi_user: bool = multi_user
 
     def prepare_message(self, session, envelope):
-        _logger.info(envelope.content)
         if envelope.smtp_utf8 and isinstance(envelope.content, (bytes, bytearray)):
             data = envelope.content
             try:
                 envelope.content = data.decode()
             except UnicodeError:
                 pass
         return super().prepare_message(session, envelope)
```

## mail_devel/resources/index.html

```diff
@@ -41,15 +41,15 @@
     </div>
 
     <div id="mailbox" class="container">
       <table>
         <thead>
           <tr>
             <th class="summary">Summary</th>
-            <th class="date">Date</th>
+            <th class="date"><span class="ordering"></span> Date</th>
             <th class="read">Read</th>
           </tr>
         </thead>
         <tbody></tbody>
         <tfoot>
           <tr id="mail-row-template" class="hidden">
             <td class="summary">
```

## mail_devel/resources/main.css

```diff
@@ -140,14 +140,21 @@
 }
 #mailbox .date, #mailbox .read {
   padding: 0 4px;
   text-align: right;
   width: 1px;
   white-space: nowrap;
 }
+#mailbox .ordering {
+  display: inline-block;
+  vertical-align: text-top;
+  width: 12pt;
+}
+#mailbox .ordering.asc:before {content: "\25B4"}
+#mailbox .ordering.desc:before {content: "\25BC"}
 
 #mailbox table th {
   border: 1px solid gray;
   background-color: var(--highlight);
   text-align: center !important;
 }
```

## mail_devel/resources/main.js

### js-beautify {}

```diff
@@ -32,29 +32,31 @@
 class MailClient {
     constructor() {
         this.users = document.getElementById("accounts");
         this.connection = document.querySelector("#connection input[type=checkbox]");
         this.mailboxes = document.getElementById("mailboxes");
         this.mailbox = document.querySelector("#mailbox table tbody");
         this.fixed_headers = ["from", "to", "cc", "bcc", "subject"];
-        this.user_name = null;
-        this.mailbox_name = null;
+        this.user_id = null;
+        this.mailbox_id = null;
         this.mail_uid = null;
         this.mail_selected = null;
         this.content_mode = "html";
         this.editor_mode = "simple";
         this.config = {};
 
         const toggle = document.querySelector("#color-scheme input");
         if (document.documentElement.classList.contains("dark"))
             toggle.checked = true;
         else if (window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches)
             toggle.checked = true
         else
             toggle.checked = false
+
+        this.reorder(false);
     }
 
     async swap_theme() {
         const toggle = document.querySelector("#color-scheme input");
         if (toggle.checked) {
             document.documentElement.classList.add("light");
             document.documentElement.classList.remove("dark");
@@ -87,28 +89,28 @@
 
         if (this.connection.checked) {
             await this.fetch_accounts();
 
             if (this.user_name)
                 await this.fetch_mailboxes(this.user_name);
 
-            if (this.mailbox_name)
-                await this.fetch_mailbox(this.mailbox_name);
+            if (this.mailbox_id)
+                await this.fetch_mailbox(this.mailbox_id);
         }
 
         setTimeout(() => {
             self.idle();
         }, 2000);
     }
 
     async set_flag(flag, method, uid = null) {
         const mail_uid = uid || this.mail_uid;
-        if (this.mailbox_name && mail_uid) {
+        if (this.mailbox_id && mail_uid) {
             await fetch(
-                `/api/${this.user_name}/${this.mailbox_name}/${mail_uid}/flags/seen`, {
+                `/api/${this.user_id}/${this.mailbox_id}/${mail_uid}/flags/seen`, {
                     method: method
                 },
             );
         }
     }
 
     async fetch_json(path) {
@@ -171,15 +173,14 @@
 
     async _mail_row_init(template, msg) {
         const self = this;
 
         const row = template.cloneNode(10);
         row.removeAttribute("id");
         row.classList.remove("hidden");
-        this.mailbox.append(row);
 
         row.querySelector(".read input").addEventListener("click", (ev) => {
             ev.preventDefault();
             ev.stopPropagation();
             self._mail_row_click(ev.target, "read");
         });
 
@@ -245,119 +246,126 @@
     async fetch_accounts() {
         const self = this;
         const data = await this.fetch_data();
         if (data === null)
             return;
 
         for (const opt of this.users.options) {
-            const idx = data.indexOf(opt.value);
-            if (idx >= 0)
-                data.splice(idx, 1);
+            const user = data[opt.value];
+            if (user !== undefined)
+                delete data[opt.value];
             else
                 opt.remove();
         }
 
-        for (const user of data)
-            this.users.add(new Option(user, user));
+        for (const uid in data)
+            this.users.add(new Option(data[uid], uid));
 
         if (this.users.selectedIndex < 0) {
             this.users.selectedIndex = 0;
             if (this.users.options[0]) {
                 await self.fetch_mailboxes(this.users.options[0].value);
             }
         } else {
             const selected = this.users.options[this.users.selectedIndex].value;
-            if (this.user_name !== selected) {
+            if (this.user_id !== selected) {
                 await self.fetch_mailboxes(selected);
             }
         }
     }
 
-    async fetch_mailboxes(user_name) {
+    async fetch_mailboxes(user_id) {
         const self = this;
-        const data = await this.fetch_data(user_name);
+        const data = await this.fetch_data(user_id);
         if (data === null)
             return;
 
-        if (this.user_name !== user_name) {
-            this.mailbox_name = null;
+        if (this.user_id !== user_id) {
+            this.mailbox_id = null;
             this.mail_uid = null;
             this.mailbox.innerHTML = "";
             this.mailboxes.selectedIndex = -1;
         }
 
-        this.user_name = user_name;
+        this.user_id = user_id;
 
         for (const opt of this.mailboxes.options) {
-            const idx = data.indexOf(opt.value);
-            if (idx >= 0)
+            const name = data[opt.uid];
+            if (name)
                 data.splice(idx, 1);
             else
                 opt.remove()
         }
 
-        for (const mailbox of data) {
-            this.mailboxes.add(new Option(mailbox, mailbox));
+        for (const uid in data) {
+            this.mailboxes.add(new Option(data[uid], uid, true, this.mailbox_id === uid));
         }
 
         if (this.mailboxes.selectedIndex < 0) {
             this.mailboxes.selectedIndex = 0;
             if (this.mailboxes.options[0]) {
                 await self.fetch_mailbox(this.mailboxes.options[0].value);
             }
         }
     }
 
-    async fetch_mailbox(mailbox_name) {
+    async fetch_mailbox(mailbox_id) {
         const self = this;
-        const data = await this.fetch_data(this.user_name, mailbox_name);
+        const data = await this.fetch_data(this.user_id, mailbox_id);
         if (data === null)
             return;
 
-        if (this.mailbox_name !== mailbox_name) {
+        if (this.mailbox_id !== mailbox_id) {
             this.mail_uid = null;
             this.mailbox.innerHTML = "";
         }
 
-        this.mailbox_name = mailbox_name;
+        this.mailbox_id = mailbox_id;
         const missing_msg = [];
         const uids = [];
+        const lines = [];
         for (const msg of data) {
             uids.push(msg.uid);
 
             let found = false;
             for (const line of this.mailbox.children) {
                 if (line.uid === msg.uid) {
                     found = true;
                     await self._mail_row_fill(line, msg);
+                    lines.push(line);
                     break;
                 }
             }
 
             if (!found)
                 missing_msg.push(msg);
         }
 
         const template = document.querySelector("#mail-row-template");
         for (const msg of missing_msg) {
             const row = await self._mail_row_init(template, msg);
 
             row.uid = msg.uid;
             await self._mail_row_fill(row, msg);
+            lines.push(row);
         }
 
-        for (const line of this.mailbox.children) {
+        for (const line of lines) {
             if (uids.indexOf(line.uid) < 0 && line !== template)
                 line.remove();
         }
+
+        if (this.sort_asc) lines.reverse();
+        for (const line of lines)
+            this.mailbox.append(line);
     }
 
     async fetch_mail(uid) {
         const self = this;
-        const data = await this.fetch_data(this.user_name, this.mailbox_name, uid);
+        const data = await this.fetch_data(this.user_id, this.mailbox_id, uid);
         if (data === null)
             return;
 
         self.mail_uid = uid;
 
         document.querySelector("#header-from input").value = data?.header?.from || "";
         document.querySelector("#header-to input").value = data?.header?.to || "";
@@ -369,15 +377,15 @@
         document.querySelector("#content iframe#html").srcdoc = data?.body_html || "";
 
         const dropdown = document.querySelector("#btn-dropdown div");
         dropdown.innerHTML = "";
 
         for (const attachment of data?.attachments || []) {
             const link = document.createElement("a");
-            link.href = `/api/${this.user_name}/${this.mailbox_name}/${uid}/attachment/${attachment}`;
+            link.href = `/api/${this.user_id}/${this.mailbox_id}/${uid}/attachment/${attachment}`;
             link.innerHTML = attachment;
             dropdown.append(link);
         }
 
         if (!data?.body_html && self.content_mode === "html")
             self.content_mode = "plain";
 
@@ -420,14 +428,31 @@
         row.append(value_td);
         row.append(btn_td);
         table.append(row);
 
         await this.visibility();
     }
 
+    async reorder(asc) {
+        this.sort_asc = asc;
+
+        const element = document.querySelector("#mailbox .date .ordering");
+        if (!element) return;
+
+        if (this.sort_asc) {
+            element.classList.add("asc");
+            element.classList.remove("desc");
+        } else {
+            element.classList.add("desc");
+            element.classList.remove("asc");
+        }
+
+        if (this.mailbox_id) await this.fetch_mailbox(this.mailbox_id);
+    }
+
     async send_mail() {
         const headers = {};
         for (const key of this.fixed_headers)
             headers[key] = document.querySelector(`#editor-${key} input`).value;
 
         for (const row of document.querySelectorAll("#editor .header .extra")) {
             const inputs = row.querySelectorAll("input");
@@ -457,19 +482,19 @@
         });
 
         document.querySelector("#editor").classList.add("hidden");
         await this.reset_editor();
     }
 
     async reply_mail() {
-        if (!this.mailbox_name || !this.mail_uid)
+        if (!this.mailbox_id || !this.mail_uid)
             return;
 
         const data = await this.fetch_data(
-            this.user_name, this.mailbox_name, this.mail_uid, "reply"
+            this.user_id, this.mailbox_id, this.mail_uid, "reply"
         );
         if (data === null)
             return;
 
         await this.reset_editor(data.header || {});
         document.querySelector("#editor").classList.remove("hidden");
     }
@@ -544,13 +569,17 @@
             ev.preventDefault();
             self.swap_theme();
         });
         document.querySelector("#uploader input").addEventListener("change", (ev) => {
             ev.preventDefault();
             self.upload_files(ev.target);
         });
+        document.querySelector("#mailbox .date").addEventListener("click", (ev) => {
+            ev.preventDefault();
+            self.reorder(!self.sort_asc);
+        });
 
         await this.load_config();
         await this.visibility();
         await this.idle();
     }
 }
```

## Comparing `mail_devel-0.8.2.dist-info/LICENSE` & `mail_devel-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mail_devel-0.8.2.dist-info/METADATA` & `mail_devel-0.9.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mail-devel
-Version: 0.8.2
+Version: 0.9.0
 Summary: IMAP and SMTP in memory test server
 Home-page: https://github.com/fkantelberg/mail-devel
 Author: Florian Kantelberg
 Author-email: florian.kantelberg@mailbox.org
 License: MIT
 Keywords: imap smtp development
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `mail_devel-0.8.2.dist-info/RECORD` & `mail_devel-0.9.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-mail_devel/__init__.py,sha256=Tk2l1KzutC4eWva0okmI2i_ZrKpPtFgQxJmH2FnxlfU,48
+mail_devel/__init__.py,sha256=qZeNBiw23A4PhC-I0tBQXtvlWUkS-HqqDbqqkU4FH9s,48
 mail_devel/__main__.py,sha256=o0YIaYqTEZeKl5v4SFUfsXWQIhuNl_15F4JF829zGC8,914
 mail_devel/auth.py,sha256=8KkFUKuipgR8RjDZL5TOzA5hQkKwDGyJIKX_-PEU604,1956
-mail_devel/http.py,sha256=p0xCNGUYu7kUsCxVwTMJOD2ACf0n-0yD-8zsZYSwPAY,13877
-mail_devel/mailbox.py,sha256=waS5nrQu7Vf183wTBUaAuE_-3wI5nx7faKOS4wMyIOw,3205
+mail_devel/http.py,sha256=TBg7_-wFXb8T37CEYBuJ_1Mt72ULZ5Z3fQmCCw0UjvI,14797
+mail_devel/mailbox.py,sha256=0HLgpXCRQ9mQPc6HMLKAvHVB-m5HmltACmGNn99Rzgw,4379
 mail_devel/service.py,sha256=3z5UqLBwjWCxXJn5Cfzt8rdU1ic92NP70AnP6IuoIKk,10918
-mail_devel/smtp.py,sha256=TEQh9xPiwUKVNwZUo3z9aPdlAXffot4OKf0ZJDEU1vs,1312
+mail_devel/smtp.py,sha256=RpxWmgyvunmQpWkCe_WoeKMBVNuqIOlCP72C1EPE8D8,1302
 mail_devel/utils.py,sha256=9ygNnIjVq6Lyz1j3hk8_S6H92P6Nf1XxcQH_cQ40Xbg,3133
 mail_devel/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mail_devel/resources/index.html,sha256=hGL654uWPN9LSUfS3LOOtVoQev_FEVLYTs7TRICVFWo,4894
-mail_devel/resources/main.css,sha256=wQIEt-ht8hsYcyjSSlaVb3Qjke6Q0EiVCoWuQkJMIm4,6160
-mail_devel/resources/main.js,sha256=PqXTePFfNnsk8wCkLi-l0JPIS_zZEq0msG0mhqZqbCw,15485
-mail_devel-0.8.2.dist-info/LICENSE,sha256=2uv3FXpGSeGfn8IfQfoIC6H2ERGw0jizs1HaWgYDMP4,1085
-mail_devel-0.8.2.dist-info/METADATA,sha256=DF28MGOPfvm9S7JTSOea7vpYkcYXvBe6IIC6Jx0dDVo,1519
-mail_devel-0.8.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-mail_devel-0.8.2.dist-info/entry_points.txt,sha256=msOFnZ8G-RwKfWNoenhoUXRX9UOkFNf-KVNSL2IQseg,56
-mail_devel-0.8.2.dist-info/top_level.txt,sha256=Q649zJRj-7u22745fgJO6Otc4d8q03ZINA6GR61x-KM,11
-mail_devel-0.8.2.dist-info/RECORD,,
+mail_devel/resources/index.html,sha256=kRVoMQLx2fUs5sI5GPVdUi6LdU4nDZo3nZfkBwBqePs,4925
+mail_devel/resources/main.css,sha256=FYEeQMIpyv2md3qd3ycf7h0rl8drwv5Rz6I-mbmQGko,6350
+mail_devel/resources/main.js,sha256=SL7ZQU5bxF6b7zG3s96FWrv1oFUwW6FKJUYTBTDaQB0,16175
+mail_devel-0.9.0.dist-info/LICENSE,sha256=2uv3FXpGSeGfn8IfQfoIC6H2ERGw0jizs1HaWgYDMP4,1085
+mail_devel-0.9.0.dist-info/METADATA,sha256=ssFRJww-NZqqfT7eNq-MR16kKFRf6aTgE9xPpB6nP-k,1519
+mail_devel-0.9.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+mail_devel-0.9.0.dist-info/entry_points.txt,sha256=msOFnZ8G-RwKfWNoenhoUXRX9UOkFNf-KVNSL2IQseg,56
+mail_devel-0.9.0.dist-info/top_level.txt,sha256=Q649zJRj-7u22745fgJO6Otc4d8q03ZINA6GR61x-KM,11
+mail_devel-0.9.0.dist-info/RECORD,,
```

