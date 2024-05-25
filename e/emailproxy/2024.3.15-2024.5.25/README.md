# Comparing `tmp/emailproxy-2024.3.15.tar.gz` & `tmp/emailproxy-2024.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailproxy-2024.3.15.tar", last modified: Fri Mar 15 08:51:07 2024, max compression
+gzip compressed data, was "emailproxy-2024.5.25.tar", last modified: Sat May 25 19:03:58 2024, max compression
```

## Comparing `emailproxy-2024.3.15.tar` & `emailproxy-2024.5.25.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:51:07.812181 emailproxy-2024.3.15/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-15 08:51:02.000000 emailproxy-2024.3.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35438 2024-03-15 08:51:07.812181 emailproxy-2024.3.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33533 2024-03-15 08:51:02.000000 emailproxy-2024.3.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:51:07.808181 emailproxy-2024.3.15/emailproxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35438 2024-03-15 08:51:07.000000 emailproxy-2024.3.15/emailproxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-15 08:51:07.000000 emailproxy-2024.3.15/emailproxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 08:51:07.000000 emailproxy-2024.3.15/emailproxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-15 08:51:07.000000 emailproxy-2024.3.15/emailproxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-15 08:51:07.000000 emailproxy-2024.3.15/emailproxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-15 08:51:07.000000 emailproxy-2024.3.15/emailproxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)   194364 2024-03-15 08:51:02.000000 emailproxy-2024.3.15/emailproxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-15 08:51:02.000000 emailproxy-2024.3.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-15 08:51:02.000000 emailproxy-2024.3.15/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-15 08:51:02.000000 emailproxy-2024.3.15/requirements-gui.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 08:51:07.812181 emailproxy-2024.3.15/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:03:58.561461 emailproxy-2024.5.25/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 19:03:53.000000 emailproxy-2024.5.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35710 2024-05-25 19:03:58.561461 emailproxy-2024.5.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33779 2024-05-25 19:03:53.000000 emailproxy-2024.5.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:03:58.561461 emailproxy-2024.5.25/emailproxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35710 2024-05-25 19:03:58.000000 emailproxy-2024.5.25/emailproxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-25 19:03:58.000000 emailproxy-2024.5.25/emailproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:03:58.000000 emailproxy-2024.5.25/emailproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-25 19:03:58.000000 emailproxy-2024.5.25/emailproxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-25 19:03:58.000000 emailproxy-2024.5.25/emailproxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 19:03:58.000000 emailproxy-2024.5.25/emailproxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   199291 2024-05-25 19:03:53.000000 emailproxy-2024.5.25/emailproxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-25 19:03:53.000000 emailproxy-2024.5.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-25 19:03:53.000000 emailproxy-2024.5.25/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-25 19:03:53.000000 emailproxy-2024.5.25/requirements-gui.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 19:03:58.561461 emailproxy-2024.5.25/setup.cfg
```

### Comparing `emailproxy-2024.3.15/LICENSE` & `emailproxy-2024.5.25/LICENSE`

 * *Files identical despite different names*

### Comparing `emailproxy-2024.3.15/PKG-INFO` & `emailproxy-2024.5.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailproxy
-Version: 2024.3.15
+Version: 2024.5.25
 Summary: Transparently add OAuth 2.0 support to IMAP/POP/SMTP clients that don't support this authentication method.
 Author-email: Simon Robinson <simon@robinson.ac>
 License: Apache License 2.0
 Project-URL: Documentation, https://github.com/simonrob/email-oauth2-proxy#email-oauth-20-proxy
 Project-URL: Release Notes, https://github.com/simonrob/email-oauth2-proxy/releases
 Project-URL: Report Issues, https://github.com/simonrob/email-oauth2-proxy/issues
 Project-URL: Source Code, https://github.com/simonrob/email-oauth2-proxy
@@ -23,14 +23,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography>=2.2
 Requires-Dist: pyasyncore; python_version >= "3.12"
 Requires-Dist: pyoslog>=0.3.0; sys_platform == "darwin"
 Requires-Dist: prompt_toolkit
+Requires-Dist: pyjwt>=2.4
 Provides-Extra: gui
 Requires-Dist: pillow; extra == "gui"
 Requires-Dist: setuptools; extra == "gui"
 Requires-Dist: timeago; extra == "gui"
 Requires-Dist: pystray>=0.19.4; extra == "gui"
 Requires-Dist: pywebview>=4.2.1; extra == "gui"
 Requires-Dist: pyobjc-framework-Cocoa; sys_platform == "darwin" and extra == "gui"
@@ -103,21 +104,21 @@
 
 If you do not have access to credentials for an existing client you will need to register your own.
 The process to do this is different for each provider, but the registration guides for several common ones are linked here.
 In all cases, when registering, make sure your client is set up to use an OAuth scope that will give it permission to access IMAP/POP/SMTP as desired.
 It is also highly recommended to use a scope that will grant "offline" access (i.e., a way to [refresh the OAuth 2.0 authentication token](https://oauth.net/2/refresh-tokens/) without user intervention).
 The [sample configuration file](https://github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) provides example scope values for several common providers.
 
-- Office 365: register a new [Microsoft identity application](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app)
+- Office 365: register a new [Microsoft identity application](https://learn.microsoft.com/entra/identity-platform/quickstart-register-app)
 - Gmail / Google Workspace: register a [Google API desktop app client](https://developers.google.com/identity/protocols/oauth2/native-app)
 - AOL and Yahoo Mail (and subproviders such as AT&T) are not currently allowing new client registrations with the OAuth email scope – the only option here is to reuse the credentials from an existing client that does have this permission.
 
 The proxy supports [Google Cloud service accounts](https://cloud.google.com/iam/docs/service-account-overview) for access to Google Workspace Gmail.
-It also supports the [client credentials grant (CCG)](https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth2-client-creds-grant-flow) and [resource owner password credentials grant (ROPCG)](https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth-ropc) OAuth 2.0 flows.
-Please note that currently only Office 365 is known to support the CCG and ROPCG methods.
+It also supports the [client credentials grant (CCG)](https://learn.microsoft.com/entra/identity-platform/v2-oauth2-client-creds-grant-flow) and [resource owner password credentials grant (ROPCG)](https://learn.microsoft.com/entra/identity-platform/v2-oauth-ropc) OAuth 2.0 flows, and [certificate credentials (JWT)](https://learn.microsoft.com/entra/identity-platform/certificate-credentials).
+Please note that currently only Office 365 is known to support the CCG, ROPCG and certificate credentials methods.
 See the [sample configuration file](https://github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) for further details.
 
 
 ## Optional arguments and configuration<a id="optional-arguments-and-configuration"></a>
 When starting the proxy there are several optional arguments that can be set to customise its behaviour.
 
 - `--no-gui` will launch the proxy without an icon, which allows it to be run as a `systemctl` service as demonstrated in [this example](https://github.com/simonrob/email-oauth2-proxy/issues/2#issuecomment-839713677), or fully headless as demonstrated in [various](https://github.com/michaelstepner/email-oauth2-proxy-aws) [other](https://github.com/blacktirion/email-oauth2-proxy-docker) subprojects.
@@ -149,14 +150,15 @@
 
 - `--log-file` allows you to specify the location of a file to send log output to (full path required).
 Log files are rotated at 32MB and 10 older log files are kept.
 This option overrides the proxy's default behaviour, which varies by platform (see [below](#troubleshooting) for details).
 
 - `--debug` enables debug mode, printing more verbose output to the log as [discussed below](#troubleshooting).
 This argument is identical to enabling debug mode from the proxy's menu bar icon.
+If needed, debug mode can also be toggled at runtime by sending the signal `SIGUSR1` (e.g.: `pkill -SIGUSR1 -f emailproxy`).
 
 ### Advanced configuration<a id="advanced-configuration"></a>
 The [example configuration file](https://github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) contains further documentation for various additional features of the proxy, including catch-all (wildcard) accounts, locally-encrypted connections and advanced Office 365 OAuth 2.0 flows.
 
 The proxy caches authenticated OAuth 2.0 tokens and associated metadata back to its own configuration file by default, but can alternatively be configured to use either a separate local file or a secrets manager service for this purpose.
 Currently only [AWS Secrets Manager](https://aws.amazon.com/secrets-manager/) is supported for remote token storage.
 To use this feature, set the [`--cache-store`](#optional-arguments-and-configuration) parameter to either a full ARN or a secret name, prefixing the value with `aws:` to identify its type to the proxy.
```

### Comparing `emailproxy-2024.3.15/README.md` & `emailproxy-2024.5.25/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,21 +65,21 @@
 
 If you do not have access to credentials for an existing client you will need to register your own.
 The process to do this is different for each provider, but the registration guides for several common ones are linked here.
 In all cases, when registering, make sure your client is set up to use an OAuth scope that will give it permission to access IMAP/POP/SMTP as desired.
 It is also highly recommended to use a scope that will grant "offline" access (i.e., a way to [refresh the OAuth 2.0 authentication token](https://oauth.net/2/refresh-tokens/) without user intervention).
 The [sample configuration file](https://github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) provides example scope values for several common providers.
 
-- Office 365: register a new [Microsoft identity application](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app)
+- Office 365: register a new [Microsoft identity application](https://learn.microsoft.com/entra/identity-platform/quickstart-register-app)
 - Gmail / Google Workspace: register a [Google API desktop app client](https://developers.google.com/identity/protocols/oauth2/native-app)
 - AOL and Yahoo Mail (and subproviders such as AT&T) are not currently allowing new client registrations with the OAuth email scope – the only option here is to reuse the credentials from an existing client that does have this permission.
 
 The proxy supports [Google Cloud service accounts](https://cloud.google.com/iam/docs/service-account-overview) for access to Google Workspace Gmail.
-It also supports the [client credentials grant (CCG)](https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth2-client-creds-grant-flow) and [resource owner password credentials grant (ROPCG)](https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth-ropc) OAuth 2.0 flows.
-Please note that currently only Office 365 is known to support the CCG and ROPCG methods.
+It also supports the [client credentials grant (CCG)](https://learn.microsoft.com/entra/identity-platform/v2-oauth2-client-creds-grant-flow) and [resource owner password credentials grant (ROPCG)](https://learn.microsoft.com/entra/identity-platform/v2-oauth-ropc) OAuth 2.0 flows, and [certificate credentials (JWT)](https://learn.microsoft.com/entra/identity-platform/certificate-credentials).
+Please note that currently only Office 365 is known to support the CCG, ROPCG and certificate credentials methods.
 See the [sample configuration file](https://github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) for further details.
 
 
 ## Optional arguments and configuration<a id="optional-arguments-and-configuration"></a>
 When starting the proxy there are several optional arguments that can be set to customise its behaviour.
 
 - `--no-gui` will launch the proxy without an icon, which allows it to be run as a `systemctl` service as demonstrated in [this example](https://github.com/simonrob/email-oauth2-proxy/issues/2#issuecomment-839713677), or fully headless as demonstrated in [various](https://github.com/michaelstepner/email-oauth2-proxy-aws) [other](https://github.com/blacktirion/email-oauth2-proxy-docker) subprojects.
@@ -111,14 +111,15 @@
 
 - `--log-file` allows you to specify the location of a file to send log output to (full path required).
 Log files are rotated at 32MB and 10 older log files are kept.
 This option overrides the proxy's default behaviour, which varies by platform (see [below](#troubleshooting) for details).
 
 - `--debug` enables debug mode, printing more verbose output to the log as [discussed below](#troubleshooting).
 This argument is identical to enabling debug mode from the proxy's menu bar icon.
+If needed, debug mode can also be toggled at runtime by sending the signal `SIGUSR1` (e.g.: `pkill -SIGUSR1 -f emailproxy`).
 
 ### Advanced configuration<a id="advanced-configuration"></a>
 The [example configuration file](https://github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) contains further documentation for various additional features of the proxy, including catch-all (wildcard) accounts, locally-encrypted connections and advanced Office 365 OAuth 2.0 flows.
 
 The proxy caches authenticated OAuth 2.0 tokens and associated metadata back to its own configuration file by default, but can alternatively be configured to use either a separate local file or a secrets manager service for this purpose.
 Currently only [AWS Secrets Manager](https://aws.amazon.com/secrets-manager/) is supported for remote token storage.
 To use this feature, set the [`--cache-store`](#optional-arguments-and-configuration) parameter to either a full ARN or a secret name, prefixing the value with `aws:` to identify its type to the proxy.
```

#### html2text {}

```diff
@@ -105,28 +105,30 @@
 when registering, make sure your client is set up to use an OAuth scope that
 will give it permission to access IMAP/POP/SMTP as desired. It is also highly
 recommended to use a scope that will grant "offline" access (i.e., a way to
 [refresh the OAuth 2.0 authentication token](https://oauth.net/2/refresh-
 tokens/) without user intervention). The [sample configuration file](https://
 github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) provides
 example scope values for several common providers. - Office 365: register a new
-[Microsoft identity application](https://learn.microsoft.com/en-us/entra/
-identity-platform/quickstart-register-app) - Gmail / Google Workspace: register
-a [Google API desktop app client](https://developers.google.com/identity/
+[Microsoft identity application](https://learn.microsoft.com/entra/identity-
+platform/quickstart-register-app) - Gmail / Google Workspace: register a
+[Google API desktop app client](https://developers.google.com/identity/
 protocols/oauth2/native-app) - AOL and Yahoo Mail (and subproviders such as
 AT&T) are not currently allowing new client registrations with the OAuth email
 scope â the only option here is to reuse the credentials from an existing
 client that does have this permission. The proxy supports [Google Cloud service
 accounts](https://cloud.google.com/iam/docs/service-account-overview) for
 access to Google Workspace Gmail. It also supports the [client credentials
-grant (CCG)](https://learn.microsoft.com/en-us/entra/identity-platform/v2-
-oauth2-client-creds-grant-flow) and [resource owner password credentials grant
-(ROPCG)](https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth-
-ropc) OAuth 2.0 flows. Please note that currently only Office 365 is known to
-support the CCG and ROPCG methods. See the [sample configuration file](https://
+grant (CCG)](https://learn.microsoft.com/entra/identity-platform/v2-oauth2-
+client-creds-grant-flow) and [resource owner password credentials grant
+(ROPCG)](https://learn.microsoft.com/entra/identity-platform/v2-oauth-ropc)
+OAuth 2.0 flows, and [certificate credentials (JWT)](https://
+learn.microsoft.com/entra/identity-platform/certificate-credentials). Please
+note that currently only Office 365 is known to support the CCG, ROPCG and
+certificate credentials methods. See the [sample configuration file](https://
 github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) for further
 details. ## Optional arguments and configuration When starting the proxy there
 are several optional arguments that can be set to customise its behaviour. - `-
 -no-gui` will launch the proxy without an icon, which allows it to be run as a
 `systemctl` service as demonstrated in [this example](https://github.com/
 simonrob/email-oauth2-proxy/issues/2#issuecomment-839713677), or fully headless
 as demonstrated in [various](https://github.com/michaelstepner/email-oauth2-
@@ -178,28 +180,30 @@
 credentials will be cached in the current configuration file. - `--log-file`
 allows you to specify the location of a file to send log output to (full path
 required). Log files are rotated at 32MB and 10 older log files are kept. This
 option overrides the proxy's default behaviour, which varies by platform (see
 [below](#troubleshooting) for details). - `--debug` enables debug mode,
 printing more verbose output to the log as [discussed below](#troubleshooting).
 This argument is identical to enabling debug mode from the proxy's menu bar
-icon. ### Advanced configuration The [example configuration file](https://
-github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) contains
-further documentation for various additional features of the proxy, including
-catch-all (wildcard) accounts, locally-encrypted connections and advanced
-Office 365 OAuth 2.0 flows. The proxy caches authenticated OAuth 2.0 tokens and
-associated metadata back to its own configuration file by default, but can
-alternatively be configured to use either a separate local file or a secrets
-manager service for this purpose. Currently only [AWS Secrets Manager](https://
-aws.amazon.com/secrets-manager/) is supported for remote token storage. To use
-this feature, set the [`--cache-store`](#optional-arguments-and-configuration)
-parameter to either a full ARN or a secret name, prefixing the value with `aws:
-` to identify its type to the proxy. You must also install the AWS SDK for
-Python: `python -m pip install boto3` and [set up authentication credentials]
-(https://boto3.amazonaws.com/v1/documentation/api/latest/guide/
+icon. If needed, debug mode can also be toggled at runtime by sending the
+signal `SIGUSR1` (e.g.: `pkill -SIGUSR1 -f emailproxy`). ### Advanced
+configuration The [example configuration file](https://github.com/simonrob/
+email-oauth2-proxy/blob/main/emailproxy.config) contains further documentation
+for various additional features of the proxy, including catch-all (wildcard)
+accounts, locally-encrypted connections and advanced Office 365 OAuth 2.0
+flows. The proxy caches authenticated OAuth 2.0 tokens and associated metadata
+back to its own configuration file by default, but can alternatively be
+configured to use either a separate local file or a secrets manager service for
+this purpose. Currently only [AWS Secrets Manager](https://aws.amazon.com/
+secrets-manager/) is supported for remote token storage. To use this feature,
+set the [`--cache-store`](#optional-arguments-and-configuration) parameter to
+either a full ARN or a secret name, prefixing the value with `aws:` to identify
+its type to the proxy. You must also install the AWS SDK for Python: `python -
+m pip install boto3` and [set up authentication credentials](https://
+boto3.amazonaws.com/v1/documentation/api/latest/guide/
 quickstart.html#configuration) (including a region). The minimum required
 permissions for the associated AWS IAM user are `secretsmanager:GetSecretValue`
 and `secretsmanager:PutSecretValue`. If the named AWS Secret does not yet
 exist, the proxy will attempt to create it; here, the `secretsmanager:
 CreateSecret` permission is also required. If you are using the proxy in a non-
 GUI environment it is possible to skip installation of dependencies that apply
 only to the interactive version. To do this, install via `python -m pip install
```

### Comparing `emailproxy-2024.3.15/emailproxy.egg-info/PKG-INFO` & `emailproxy-2024.5.25/emailproxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailproxy
-Version: 2024.3.15
+Version: 2024.5.25
 Summary: Transparently add OAuth 2.0 support to IMAP/POP/SMTP clients that don't support this authentication method.
 Author-email: Simon Robinson <simon@robinson.ac>
 License: Apache License 2.0
 Project-URL: Documentation, https://github.com/simonrob/email-oauth2-proxy#email-oauth-20-proxy
 Project-URL: Release Notes, https://github.com/simonrob/email-oauth2-proxy/releases
 Project-URL: Report Issues, https://github.com/simonrob/email-oauth2-proxy/issues
 Project-URL: Source Code, https://github.com/simonrob/email-oauth2-proxy
@@ -23,14 +23,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography>=2.2
 Requires-Dist: pyasyncore; python_version >= "3.12"
 Requires-Dist: pyoslog>=0.3.0; sys_platform == "darwin"
 Requires-Dist: prompt_toolkit
+Requires-Dist: pyjwt>=2.4
 Provides-Extra: gui
 Requires-Dist: pillow; extra == "gui"
 Requires-Dist: setuptools; extra == "gui"
 Requires-Dist: timeago; extra == "gui"
 Requires-Dist: pystray>=0.19.4; extra == "gui"
 Requires-Dist: pywebview>=4.2.1; extra == "gui"
 Requires-Dist: pyobjc-framework-Cocoa; sys_platform == "darwin" and extra == "gui"
@@ -103,21 +104,21 @@
 
 If you do not have access to credentials for an existing client you will need to register your own.
 The process to do this is different for each provider, but the registration guides for several common ones are linked here.
 In all cases, when registering, make sure your client is set up to use an OAuth scope that will give it permission to access IMAP/POP/SMTP as desired.
 It is also highly recommended to use a scope that will grant "offline" access (i.e., a way to [refresh the OAuth 2.0 authentication token](https://oauth.net/2/refresh-tokens/) without user intervention).
 The [sample configuration file](https://github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) provides example scope values for several common providers.
 
-- Office 365: register a new [Microsoft identity application](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app)
+- Office 365: register a new [Microsoft identity application](https://learn.microsoft.com/entra/identity-platform/quickstart-register-app)
 - Gmail / Google Workspace: register a [Google API desktop app client](https://developers.google.com/identity/protocols/oauth2/native-app)
 - AOL and Yahoo Mail (and subproviders such as AT&T) are not currently allowing new client registrations with the OAuth email scope – the only option here is to reuse the credentials from an existing client that does have this permission.
 
 The proxy supports [Google Cloud service accounts](https://cloud.google.com/iam/docs/service-account-overview) for access to Google Workspace Gmail.
-It also supports the [client credentials grant (CCG)](https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth2-client-creds-grant-flow) and [resource owner password credentials grant (ROPCG)](https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth-ropc) OAuth 2.0 flows.
-Please note that currently only Office 365 is known to support the CCG and ROPCG methods.
+It also supports the [client credentials grant (CCG)](https://learn.microsoft.com/entra/identity-platform/v2-oauth2-client-creds-grant-flow) and [resource owner password credentials grant (ROPCG)](https://learn.microsoft.com/entra/identity-platform/v2-oauth-ropc) OAuth 2.0 flows, and [certificate credentials (JWT)](https://learn.microsoft.com/entra/identity-platform/certificate-credentials).
+Please note that currently only Office 365 is known to support the CCG, ROPCG and certificate credentials methods.
 See the [sample configuration file](https://github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) for further details.
 
 
 ## Optional arguments and configuration<a id="optional-arguments-and-configuration"></a>
 When starting the proxy there are several optional arguments that can be set to customise its behaviour.
 
 - `--no-gui` will launch the proxy without an icon, which allows it to be run as a `systemctl` service as demonstrated in [this example](https://github.com/simonrob/email-oauth2-proxy/issues/2#issuecomment-839713677), or fully headless as demonstrated in [various](https://github.com/michaelstepner/email-oauth2-proxy-aws) [other](https://github.com/blacktirion/email-oauth2-proxy-docker) subprojects.
@@ -149,14 +150,15 @@
 
 - `--log-file` allows you to specify the location of a file to send log output to (full path required).
 Log files are rotated at 32MB and 10 older log files are kept.
 This option overrides the proxy's default behaviour, which varies by platform (see [below](#troubleshooting) for details).
 
 - `--debug` enables debug mode, printing more verbose output to the log as [discussed below](#troubleshooting).
 This argument is identical to enabling debug mode from the proxy's menu bar icon.
+If needed, debug mode can also be toggled at runtime by sending the signal `SIGUSR1` (e.g.: `pkill -SIGUSR1 -f emailproxy`).
 
 ### Advanced configuration<a id="advanced-configuration"></a>
 The [example configuration file](https://github.com/simonrob/email-oauth2-proxy/blob/main/emailproxy.config) contains further documentation for various additional features of the proxy, including catch-all (wildcard) accounts, locally-encrypted connections and advanced Office 365 OAuth 2.0 flows.
 
 The proxy caches authenticated OAuth 2.0 tokens and associated metadata back to its own configuration file by default, but can alternatively be configured to use either a separate local file or a secrets manager service for this purpose.
 Currently only [AWS Secrets Manager](https://aws.amazon.com/secrets-manager/) is supported for remote token storage.
 To use this feature, set the [`--cache-store`](#optional-arguments-and-configuration) parameter to either a full ARN or a secret name, prefixing the value with `aws:` to identify its type to the proxy.
```

### Comparing `emailproxy-2024.3.15/emailproxy.py` & `emailproxy-2024.5.25/emailproxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """A simple IMAP/POP/SMTP proxy that intercepts authenticate and login commands, transparently replacing them with OAuth
 2.0 authentication. Designed for apps/clients that don't support OAuth 2.0 but need to connect to modern servers."""
 
 __author__ = 'Simon Robinson'
 __copyright__ = 'Copyright (c) 2024 Simon Robinson'
 __license__ = 'Apache 2.0'
-__version__ = '2024-03-15'  # ISO 8601 (YYYY-MM-DD)
+__version__ = '2024-05-25'  # ISO 8601 (YYYY-MM-DD)
 __package_version__ = '.'.join([str(int(i)) for i in __version__.split('-')])  # for pyproject.toml usage only
 
 import abc
 import argparse
 import base64
 import binascii
 import configparser
@@ -172,14 +172,15 @@
 
 # seconds to wait before cancelling authentication requests (i.e., the user has this long to log in) - note that the
 # actual server timeout is often around 60 seconds, so the connection may be closed in the background and immediately
 # disconnect after login completes; however, the login credentials will still be saved and used for future requests
 AUTHENTICATION_TIMEOUT = 600
 
 TOKEN_EXPIRY_MARGIN = 600  # seconds before its expiry to refresh the OAuth 2.0 token
+JWT_LIFETIME = 300  # seconds to add to the current time and use for the `exp` value in JWT certificate credentials
 
 LOG_FILE_MAX_SIZE = 32 * 1024 * 1024  # when using a log file, its maximum size in bytes before rollover (0 = no limit)
 LOG_FILE_MAX_BACKUPS = 10  # the number of log files to keep when LOG_FILE_MAX_SIZE is exceeded (0 = disable rollover)
 
 IMAP_TAG_PATTERN = r'[!#$&\',-\[\]-z|}~]+'  # https://ietf.org/rfc/rfc9051.html#name-formal-syntax
 IMAP_AUTHENTICATION_REQUEST_MATCHER = re.compile('^(?P<tag>%s) (?P<command>(LOGIN|AUTHENTICATE)) '
                                                  '(?P<flags>.*)$' % IMAP_TAG_PATTERN, flags=re.IGNORECASE)
@@ -709,14 +710,16 @@
         redirect_uri = AppConfig.get_option_with_catch_all_fallback(config, username, 'redirect_uri')
         redirect_listen_address = AppConfig.get_option_with_catch_all_fallback(config, username,
                                                                                'redirect_listen_address')
         client_id = AppConfig.get_option_with_catch_all_fallback(config, username, 'client_id')
         client_secret = AppConfig.get_option_with_catch_all_fallback(config, username, 'client_secret')
         client_secret_encrypted = AppConfig.get_option_with_catch_all_fallback(config, username,
                                                                                'client_secret_encrypted')
+        jwt_certificate_path = AppConfig.get_option_with_catch_all_fallback(config, username, 'jwt_certificate_path')
+        jwt_key_path = AppConfig.get_option_with_catch_all_fallback(config, username, 'jwt_key_path')
 
         # note that we don't require permission_url here because it is not needed for the client credentials grant flow,
         # and likewise for client_secret here because it can be optional for Office 365 configurations
         if not (token_url and oauth2_scope and redirect_uri and client_id):
             Log.error('Proxy config file entry incomplete for account', username, '- aborting login')
             return (False, '%s: Incomplete config file entry found for account %s - please make sure all required '
                            'fields are added (permission_url, token_url, oauth2_scope, redirect_uri, client_id '
@@ -762,26 +765,69 @@
         try:
             # if both secret values are present we use the unencrypted version (as it may have been user-edited)
             if client_secret_encrypted:
                 if not client_secret:
                     try:
                         client_secret = cryptographer.decrypt(client_secret_encrypted)
                     except InvalidToken as e:  # needed to avoid looping (we don't remove secrets on decryption failure)
-                        Log.error('Invalid password to decrypt', username, 'secret - aborting login:',
-                                  Log.error_string(e))
+                        Log.error('Invalid password to decrypt `client_secret_encrypted` for account', username,
+                                  '- aborting login:', Log.error_string(e))
                         return False, '%s: Login failed - the password for account %s is incorrect' % (
                             APP_NAME, username)
                 else:
                     Log.info('Warning: found both `client_secret_encrypted` and `client_secret` for account', username,
-                             ' - the un-encrypted value will be used. Removing the un-encrypted value is recommended')
+                             '- the un-encrypted value will be used. Removing the un-encrypted value is recommended')
+
+            # O365 certificate credentials - see: learn.microsoft.com/entra/identity-platform/certificate-credentials
+            jwt_client_assertion = None
+            if jwt_certificate_path and jwt_key_path:
+                if client_secret or client_secret_encrypted:
+                    client_secret_type = '`client_secret%s`' % ('_encrypted' if client_secret_encrypted else '')
+                    Log.info('Warning: found both certificate credentials and', client_secret_type, 'for account',
+                             username, '- the', client_secret_type, 'value will be used. To use certificate',
+                             'credentials, remove the client secret value')
+
+                else:
+                    try:
+                        # noinspection PyUnresolvedReferences
+                        import jwt
+                    except ImportError:
+                        return False, ('Unable to load jwt, which is a requirement when using certificate credentials '
+                                       '(`jwt_` options). Please run `python -m pip install -r requirements-core.txt`')
+                    import uuid
+                    from cryptography import x509
+                    from cryptography.hazmat.primitives import serialization
+
+                    try:
+                        jwt_now = datetime.datetime.now(datetime.timezone.utc)
+                        jwt_certificate_fingerprint = x509.load_pem_x509_certificate(
+                            pathlib.Path(jwt_certificate_path).read_bytes()).fingerprint(hashes.SHA256())
+                        jwt_client_assertion = jwt.encode(
+                            {
+                                'aud': token_url,
+                                'exp': jwt_now + datetime.timedelta(seconds=JWT_LIFETIME),
+                                'iss': client_id,
+                                'jti': str(uuid.uuid4()),
+                                'nbf': jwt_now,
+                                'sub': client_id
+                            },
+                            serialization.load_pem_private_key(pathlib.Path(jwt_key_path).read_bytes(), password=None),
+                            algorithm='RS256',
+                            headers={
+                                'x5t#S256': base64.urlsafe_b64encode(jwt_certificate_fingerprint).decode('utf-8')
+                            })
+                    except FileNotFoundError:
+                        return (False, 'Unable to create credentials assertion for account %s - please check that the '
+                                       '`jwt_certificate_path` and `jwt_key_path` values are correct' % username)
 
             if access_token or refresh_token:  # if possible, refresh the existing token(s)
                 if not access_token or access_token_expiry - current_time < TOKEN_EXPIRY_MARGIN:
                     if refresh_token:
                         response = OAuth2Helper.refresh_oauth2_access_token(token_url, client_id, client_secret,
+                                                                            jwt_client_assertion, username,
                                                                             cryptographer.decrypt(refresh_token))
 
                         access_token = response['access_token']
                         config.set(username, 'access_token', cryptographer.encrypt(access_token))
                         config.set(username, 'access_token_expiry', str(current_time + response['expires_in']))
                         if 'refresh_token' in response:
                             config.set(username, 'refresh_token', cryptographer.encrypt(response['refresh_token']))
@@ -807,26 +853,27 @@
                                                                                   client_id, oauth2_scope, username)
 
                     # note: get_oauth2_authorisation_code is a blocking call (waiting on user to provide code)
                     success, auth_result = OAuth2Helper.get_oauth2_authorisation_code(permission_url, redirect_uri,
                                                                                       redirect_listen_address, username)
 
                     if not success:
-                        Log.info('Authorisation result error for', username, '- aborting login.', auth_result)
+                        Log.info('Authorisation result error for account', username, '- aborting login.', auth_result)
                         return False, '%s: Login failed for account %s: %s' % (APP_NAME, username, auth_result)
 
                 if not oauth2_flow:
-                    Log.error('No `oauth2_flow` value specified for', username, '- aborting login')
+                    Log.error('No `oauth2_flow` value specified for account', username, '- aborting login')
                     return (False, '%s: Incomplete config file entry found for account %s - please make sure an '
                                    '`oauth2_flow` value is specified when using a method that does not require a '
                                    '`permission_url`' % (APP_NAME, username))
 
                 response = OAuth2Helper.get_oauth2_authorisation_tokens(token_url, redirect_uri, client_id,
-                                                                        client_secret, auth_result, oauth2_scope,
-                                                                        oauth2_flow, username, password)
+                                                                        client_secret, jwt_client_assertion,
+                                                                        auth_result, oauth2_scope, oauth2_flow,
+                                                                        username, password)
 
                 if AppConfig.get_global('encrypt_client_secret_on_first_use', fallback=False):
                     if client_secret:
                         # note: save to the `username` entry even if `user_domain` exists, avoiding conflicts when
                         # using `encrypt_client_secret_on_first_use` with the `allow_catch_all_accounts` option
                         config.set(username, 'client_secret_encrypted', cryptographer.encrypt(client_secret))
                         config.remove_option(username, 'client_secret')
@@ -839,16 +886,17 @@
                 config.set(username, 'token_iterations', str(cryptographer.iterations))
                 config.set(username, 'access_token', cryptographer.encrypt(access_token))
                 config.set(username, 'access_token_expiry', str(current_time + response['expires_in']))
 
                 if 'refresh_token' in response:
                     config.set(username, 'refresh_token', cryptographer.encrypt(response['refresh_token']))
                 elif permission_url:  # ignore this situation with CCG/ROPCG/service account flows - it is expected
-                    Log.info('Warning: no refresh token returned for', username, '- you will need to re-authenticate',
-                             'each time the access token expires (does your `oauth2_scope` value allow `offline` use?)')
+                    Log.info('Warning: no refresh token returned for account', username, '- you will need to',
+                             're-authenticate each time the access token expires (does your `oauth2_scope` value allow',
+                             '`offline` use?)')
 
                 AppConfig.save()
 
             # send authentication command to server (response checked in ServerConnection) - note: we only support
             # single-trip authentication (SASL) without actually checking the server's capabilities - improve?
             oauth2_string = OAuth2Helper.construct_oauth2_string(username, access_token)
             return True, oauth2_string
@@ -863,15 +911,15 @@
                 # if this is already a second failure, remove the refresh token as well, and force re-authentication
                 config.remove_option(username, 'token_salt')
                 config.remove_option(username, 'token_iterations')
                 config.remove_option(username, 'refresh_token')
 
             AppConfig.save()
 
-            Log.info('Retrying login due to exception while refreshing OAuth 2.0 tokens for', username,
+            Log.info('Retrying login due to exception while refreshing access token for account', username,
                      '(attempt %d):' % (1 if has_access_token else 2), Log.error_string(e))
             return OAuth2Helper.get_oauth2_credentials(username, password, reload_remote_accounts=False)
 
         except InvalidToken as e:
             # regardless of the `delete_account_token_on_password_error` setting, we only reset tokens for standard or
             # ROPCG flows; when using CCG or a service account it is far safer to deny account access and require a
             # config file edit in order to reset an account rather than allowing *any* password to be used for access
@@ -880,28 +928,30 @@
                 config.remove_option(username, 'access_token')
                 config.remove_option(username, 'access_token_expiry')
                 config.remove_option(username, 'token_salt')
                 config.remove_option(username, 'token_iterations')
                 config.remove_option(username, 'refresh_token')
                 AppConfig.save()
 
-                Log.info('Retrying login due to exception while decrypting OAuth 2.0 credentials for', username,
+                Log.info('Retrying login due to exception while decrypting OAuth 2.0 credentials for account', username,
                          '(invalid password):', Log.error_string(e))
                 return OAuth2Helper.get_oauth2_credentials(username, password, reload_remote_accounts=False)
 
-            Log.error('Invalid password to decrypt', username, 'credentials - aborting login:', Log.error_string(e))
+            Log.error('Invalid password to decrypt credentials for account', username, '- aborting login:',
+                      Log.error_string(e))
             return False, '%s: Login failed - the password for account %s is incorrect' % (APP_NAME, username)
 
         except Exception as e:
             # note that we don't currently remove cached credentials here, as failures on the initial request are before
             # caching happens, and the assumption is that refresh token request exceptions are temporal (e.g., network
             # errors: URLError(OSError(50, 'Network is down'))) - access token 400 Bad Request HTTPErrors with messages
             # such as 'authorisation code was already redeemed' are caused by our support for simultaneous requests,
             # and will work from the next request; however, please report an issue if you encounter problems here
-            Log.info('Caught exception while requesting OAuth 2.0 credentials for %s:' % username, Log.error_string(e))
+            Log.info('Caught exception while requesting OAuth 2.0 credentials for account %s:' % username,
+                     Log.error_string(e))
             return False, '%s: Login failed for account %s - please check your internet connection and retry' % (
                 APP_NAME, username)
 
     @staticmethod
     def oauth2_url_escape(text):
         return urllib.parse.quote(text, safe='~-._')  # see https://tools.ietf.org/html/rfc3986#section-2.3
 
@@ -1010,15 +1060,15 @@
                 response_queue_reference.put(QUEUE_SENTINEL)  # make sure all watchers exit
                 return False, '%s is shutting down' % APP_NAME
 
             if data['permission_url'] == permission_url and data['username'] == username:  # a response meant for us
                 # to improve no-GUI mode we also support the use of a local redirection receiver server or terminal
                 # entry to authenticate; this result is a timeout, wsgi request error/failure, or terminal auth ctrl+c
                 if 'expired' in data and data['expired']:
-                    return False, 'No-GUI authorisation request failed or timed out'
+                    return False, 'No-GUI authorisation request failed or timed out for account %s' % data['username']
 
                 if 'local_server_auth' in data:
                     threading.Thread(target=OAuth2Helper.start_redirection_receiver_server, args=(data,),
                                      name='EmailOAuth2Proxy-auth-%s' % data['username'], daemon=True).start()
 
                 else:
                     if 'response_url' in data and OAuth2Helper.match_redirect_uri(token_request['redirect_uri'],
@@ -1027,54 +1077,63 @@
                         # as IntelliJ has a bug incorrectly detecting parse_qs/l as returning a dict with byte-type keys
                         response = {str(key): value for key, value in
                                     urllib.parse.parse_qsl(urllib.parse.urlparse(data['response_url']).query)}
                         if 'code' in response and response['code']:
                             authorisation_code = OAuth2Helper.oauth2_url_unescape(response['code'])
                             if authorisation_code:
                                 return True, authorisation_code
-                            return False, 'No OAuth 2.0 authorisation code returned'
+                            return False, 'No OAuth 2.0 authorisation code returned for account %s' % data['username']
                         if 'error' in response:
-                            message = 'OAuth 2.0 authorisation error: %s' % response['error']
+                            message = 'OAuth 2.0 authorisation error for account %s: ' % data['username']
+                            message += response['error']
                             message += '; %s' % response['error_description'] if 'error_description' in response else ''
                             return False, message
-                        return False, 'OAuth 2.0 authorisation response has no code or error message'
-                    return False, 'OAuth 2.0 authorisation response is missing or does not match `redirect_uri`'
+                        return (False, 'OAuth 2.0 authorisation response for account %s has neither code nor error '
+                                       'message' % data['username'])
+                    return (False, 'OAuth 2.0 authorisation response for account %s is missing or does not match'
+                                   '`redirect_uri`' % data['username'])
 
             else:  # not for this thread - put back into queue
                 response_queue_reference.put(data)
                 time.sleep(1)
 
     @staticmethod
-    def get_oauth2_authorisation_tokens(token_url, redirect_uri, client_id, client_secret, authorisation_code,
-                                        oauth2_scope, oauth2_flow, username, password):
+    def get_oauth2_authorisation_tokens(token_url, redirect_uri, client_id, client_secret, jwt_client_assertion,
+                                        authorisation_code, oauth2_scope, oauth2_flow, username, password):
         """Requests OAuth 2.0 access and refresh tokens from token_url using the given client_id, client_secret,
         authorisation_code and redirect_uri, returning a dict with 'access_token', 'expires_in', and 'refresh_token'
         on success, or throwing an exception on failure (e.g., HTTP 400)"""
         if oauth2_flow == 'service_account':  # service accounts are slightly different, and are handled separately
             return OAuth2Helper.get_service_account_authorisation_token(client_id, client_secret, oauth2_scope,
                                                                         username)
 
         params = {'client_id': client_id, 'client_secret': client_secret, 'code': authorisation_code,
                   'redirect_uri': redirect_uri, 'grant_type': oauth2_flow}
         if not client_secret:
             del params['client_secret']  # client secret can be optional for O365, but we don't want a None entry
+
+            # certificate credentials are only used when no client secret is provided
+            if jwt_client_assertion:
+                params['client_assertion_type'] = 'urn:ietf:params:oauth:client-assertion-type:jwt-bearer'
+                params['client_assertion'] = jwt_client_assertion
+
         if oauth2_flow != 'authorization_code':
             del params['code']  # CCG/ROPCG flows have no code, but we need the scope and (for ROPCG) username+password
             params['scope'] = oauth2_scope
             if oauth2_flow == 'password':
                 params['username'] = username
                 params['password'] = password
         try:
             response = urllib.request.urlopen(
                 urllib.request.Request(token_url, data=urllib.parse.urlencode(params).encode('utf-8'),
                                        headers={'User-Agent': APP_NAME}), timeout=AUTHENTICATION_TIMEOUT).read()
             return json.loads(response)
         except urllib.error.HTTPError as e:
             e.message = json.loads(e.read())
-            Log.debug('Error requesting access token - received invalid response:', e.message)
+            Log.debug('Error requesting access token for account', username, '- received invalid response:', e.message)
             raise e
 
     # noinspection PyUnresolvedReferences
     @staticmethod
     def get_service_account_authorisation_token(key_type, key_path_or_contents, oauth2_scope, username):
         """Requests an authorisation token via a Service Account key (currently Google Cloud only)"""
         import json
@@ -1083,49 +1142,60 @@
             import google.oauth2.service_account
             import google.auth.transport.requests
         except ModuleNotFoundError:
             raise Exception('Unable to load Google Auth SDK - please install the `requests` and `google-auth` modules: '
                             '`python -m pip install requests google-auth`')
 
         if key_type == 'file':
-            with open(key_path_or_contents) as key_file:
-                service_account = json.load(key_file)
+            try:
+                with open(key_path_or_contents) as key_file:
+                    service_account = json.load(key_file)
+            except IOError as e:
+                raise FileNotFoundError('Unable to open service account key file %s for account %s',
+                                        (key_path_or_contents, username)) from e
         elif key_type == 'key':
             service_account = json.loads(key_path_or_contents)
         else:
-            raise Exception('Service account key type not specified - `client_id` must be set to `file` or `key`')
+            raise Exception('Service account key type not specified for account %s - `client_id` must be set to '
+                            '`file` or `key`' % username)
 
         credentials = google.oauth2.service_account.Credentials.from_service_account_info(service_account)
         credentials = credentials.with_scopes(oauth2_scope.split(' '))
         credentials = credentials.with_subject(username)
 
         request = google.auth.transport.requests.Request()
         credentials.refresh(request)
         return {'access_token': credentials.token, 'expires_in': int(credentials.expiry.timestamp() - time.time())}
 
     @staticmethod
-    def refresh_oauth2_access_token(token_url, client_id, client_secret, refresh_token):
+    def refresh_oauth2_access_token(token_url, client_id, client_secret, jwt_client_assertion, username, refresh_token):
         """Obtains a new access token from token_url using the given client_id, client_secret and refresh token,
         returning a dict with 'access_token', 'expires_in', and 'refresh_token' on success; exception on failure"""
         params = {'client_id': client_id, 'client_secret': client_secret, 'refresh_token': refresh_token,
                   'grant_type': 'refresh_token'}
         if not client_secret:
             del params['client_secret']  # client secret can be optional for O365, but we don't want a None entry
+
+            # certificate credentials are only used when no client secret is provided
+            if jwt_client_assertion:
+                params['client_assertion_type'] = 'urn:ietf:params:oauth:client-assertion-type:jwt-bearer'
+                params['client_assertion'] = jwt_client_assertion
+
         try:
             response = urllib.request.urlopen(
                 urllib.request.Request(token_url, data=urllib.parse.urlencode(params).encode('utf-8'),
                                        headers={'User-Agent': APP_NAME}), timeout=AUTHENTICATION_TIMEOUT).read()
             token = json.loads(response)
             if 'expires_in' in token:  # some servers return integer values as strings - fix expiry values (GitHub #237)
                 token['expires_in'] = int(token['expires_in'])
             return token
 
         except urllib.error.HTTPError as e:
             e.message = json.loads(e.read())
-            Log.debug('Error refreshing access token - received invalid response:', e.message)
+            Log.debug('Error refreshing access token for account', username, '- received invalid response:', e.message)
             if e.code == 400:  # 400 Bad Request typically means re-authentication is required (token expired)
                 raise OAuth2Helper.TokenRefreshError from e
             raise e
 
     @staticmethod
     def construct_oauth2_string(username, access_token):
         """Constructs an OAuth 2.0 SASL authentication string from the given username and access token"""
@@ -2627,15 +2697,15 @@
         # fix pystray <= 0.19.4 incompatibility with PIL 10.0.0+; resolved in 0.19.5 and later via pystray PR #147
         with warnings.catch_warnings():
             warnings.simplefilter('ignore', DeprecationWarning)
             pystray_version = pkg_resources.get_distribution('pystray').version
             pillow_version = pkg_resources.get_distribution('pillow').version
             if pkg_resources.parse_version(pystray_version) <= pkg_resources.parse_version('0.19.4') and \
                     pkg_resources.parse_version(pillow_version) >= pkg_resources.parse_version('10.0.0'):
-                Image.ANTIALIAS = Image.LANCZOS
+                Image.ANTIALIAS = Image.LANCZOS if hasattr(Image, 'LANCZOS') else Image.Resampling.LANCZOS
         icon_class = RetinaIcon if sys.platform == 'darwin' else pystray.Icon
         return icon_class(APP_NAME, App.get_image(), APP_NAME, menu=pystray.Menu(
             pystray.MenuItem('Servers and accounts', pystray.Menu(self.create_config_menu)),
             pystray.MenuItem('Authorise account', pystray.Menu(self.create_authorisation_menu)),
             pystray.Menu.SEPARATOR,
             pystray.MenuItem('Start at login', self.toggle_start_at_login, checked=self.started_at_login),
             pystray.MenuItem('Debug mode', lambda _, item: self.toggle_debug(not item.checked),
@@ -2832,16 +2902,18 @@
             authorisation_window = webview.create_window(window_title, html=auth_page, on_top=True, text_select=True)
         else:
             authorisation_window = webview.create_window(window_title, request['permission_url'], on_top=True)
         setattr(authorisation_window, 'get_title', lambda window: window.title)  # add missing get_title method
 
         # pywebview 3.6+ moved window events to a separate namespace in a non-backwards-compatible way
         # noinspection PyDeprecation
-        if pkg_resources.parse_version(
-                pkg_resources.get_distribution('pywebview').version) < pkg_resources.parse_version('3.6'):
+        pywebview_version = pkg_resources.parse_version(pkg_resources.get_distribution('pywebview').version)
+        # the version zero check is due to a bug in the Ubuntu 22.04 python-pywebview package - see GitHub #242
+        # noinspection PyDeprecation
+        if pkg_resources.parse_version('0') < pywebview_version < pkg_resources.parse_version('3.6'):
             # noinspection PyUnresolvedReferences
             authorisation_window.loaded += self.authorisation_window_loaded
         else:
             authorisation_window.events.loaded += self.authorisation_window_loaded
 
     def handle_authorisation_windows(self):
         if sys.platform != 'darwin':
```

### Comparing `emailproxy-2024.3.15/pyproject.toml` & `emailproxy-2024.5.25/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61.0", "pyasyncore; python_version >= '3.12'", "cryptography"] # core requirements are needed for version detection, which requires importing the script
+requires = ["setuptools>=61.0", "pyasyncore; python_version >= '3.12'", "cryptography"] # core requirements are needed for version detection when building for PyPI, which requires importing (but not running) the script on `ubuntu-latest`
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "emailproxy"
 authors = [
     { name = "Simon Robinson", email = "simon@robinson.ac" }
 ]
```

### Comparing `emailproxy-2024.3.15/requirements-core.txt` & `emailproxy-2024.5.25/requirements-core.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,7 +9,10 @@
 pyasyncore; python_version >= '3.12'
 
 # macOS only: output to unified logging
 pyoslog>=0.3.0; sys_platform == 'darwin'
 
 # required only if using the --external-auth option in --no-gui mode
 prompt_toolkit
+
+# required only if using JWT certificate credentials (O365)
+pyjwt>=2.4
```

### Comparing `emailproxy-2024.3.15/requirements-gui.txt` & `emailproxy-2024.5.25/requirements-gui.txt`

 * *Files identical despite different names*

