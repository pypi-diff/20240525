# Comparing `tmp/agency_swarm-0.2.1.tar.gz` & `tmp/agency_swarm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency_swarm-0.2.1.tar", last modified: Sat Apr 27 02:28:06 2024, max compression
+gzip compressed data, was "agency_swarm-0.2.2.tar", last modified: Thu May  9 05:41:22 2024, max compression
```

## Comparing `agency_swarm-0.2.1.tar` & `agency_swarm-0.2.2.tar`

### file list

```diff
@@ -1,191 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.887431 agency_swarm-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.851431 agency_swarm-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.859431 agency_swarm-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/.github/workflows/close-issues.yml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-04-27 02:28:06.887431 agency_swarm-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.859431 agency_swarm-0.2.1/agency_swarm/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.863431 agency_swarm-0.2.1/agency_swarm/agency/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46496 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/agency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.863431 agency_swarm-0.2.1/agency_swarm/agency/genesis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.863431 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/AgentCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.863431 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.863431 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisAgency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.863431 agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.867431 agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.867431 agency_swarm-0.2.1/agency_swarm/agency/genesis/OpenAPICreator/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/OpenAPICreator/OpenAPICreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/OpenAPICreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/OpenAPICreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.867431 agency_swarm-0.2.1/agency_swarm/agency/genesis/OpenAPICreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.867431 agency_swarm-0.2.1/agency_swarm/agency/genesis/ToolCreator/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/ToolCreator/ToolCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/ToolCreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/ToolCreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.867431 agency_swarm-0.2.1/agency_swarm/agency/genesis/ToolCreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/manifesto.md
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agency/genesis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.867431 agency_swarm-0.2.1/agency_swarm/agents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.867431 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/instructions.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.871431 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/GoBack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/Scroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.871431 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/util/get_b64_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.871431 agency_swarm-0.2.1/agency_swarm/agents/Devid/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/Devid.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.875431 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/ChangeFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/CheckCurrentDir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/CommandExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/DirectoryNavigator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/FileMover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/FileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/FileWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/ListDir.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.875431 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/util/format_file_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30562 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/agents/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.875431 agency_swarm-0.2.1/agency_swarm/messages/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/messages/message_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.875431 agency_swarm-0.2.1/agency_swarm/threads/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/threads/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/threads/thread_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.875431 agency_swarm-0.2.1/agency_swarm/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/tools/BaseTool.py
--rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/tools/ToolFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.875431 agency_swarm-0.2.1/agency_swarm/tools/oai/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/tools/oai/CodeInterpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/tools/oai/FileSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/tools/oai/Retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/tools/oai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.875431 agency_swarm-0.2.1/agency_swarm/user/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/user/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.879431 agency_swarm-0.2.1/agency_swarm/util/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.879431 agency_swarm-0.2.1/agency_swarm/util/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/cli/create_agent_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/cli/import_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.879431 agency_swarm-0.2.1/agency_swarm/util/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/helpers/get_available_agent_descriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/helpers/list_available_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/oai.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/agency_swarm/util/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.887431 agency_swarm-0.2.1/agency_swarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-04-27 02:28:06.000000 agency_swarm-0.2.1/agency_swarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-27 02:28:06.000000 agency_swarm-0.2.1/agency_swarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 02:28:06.000000 agency_swarm-0.2.1/agency_swarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-27 02:28:06.000000 agency_swarm-0.2.1/agency_swarm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-27 02:28:06.000000 agency_swarm-0.2.1/agency_swarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 02:28:06.000000 agency_swarm-0.2.1/agency_swarm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.879431 agency_swarm-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.879431 agency_swarm-0.2.1/docs/advanced-usage/
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/advanced-usage/agencies.md
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/advanced-usage/agents.md
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/advanced-usage/azure-openai.md
--rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/advanced-usage/tools.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/deployment.md
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.879431 agency_swarm-0.2.1/docs/introduction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/introduction/showcase.md
--rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/docs/quick_start.md
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.883431 agency_swarm-0.2.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    49298 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/notebooks/Agency_Swarm_with_Open_Source_Model.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/notebooks/agency_async.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/notebooks/azure.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/notebooks/genesis_agency.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/notebooks/web_browser_agent.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 02:28:06.887431 agency_swarm-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.883431 agency_swarm-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.855431 agency_swarm-0.2.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.883431 agency_swarm-0.2.1/tests/data/files/
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/files/csv-test.csv
--rw-r--r--   0 runner    (1001) docker     (127)   102408 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/files/generated_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/files/test-docx.docx
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/files/test-html.html
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/files/test-md.md
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/files/test-pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/files/test-txt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/files/test-xml.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.883431 agency_swarm-0.2.1/tests/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/schemas/ga4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/schemas/get-headers-params.json
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/schemas/get-weather.json
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/schemas/relevance.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.883431 agency_swarm-0.2.1/tests/data/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/data/tools/ExampleTool1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:28:06.887431 agency_swarm-0.2.1/tests/demos/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/demos/demo_gradio.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/demos/streaming_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/demos/term_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    19817 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/test_agency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-27 02:27:56.000000 agency_swarm-0.2.1/tests/test_tool_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.148850 agency_swarm-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.112850 agency_swarm-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.120850 agency_swarm-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/.github/workflows/close-issues.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-05-09 05:41:22.148850 agency_swarm-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.120850 agency_swarm-0.2.2/agency_swarm/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.124850 agency_swarm-0.2.2/agency_swarm/agency/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46807 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/agency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.124850 agency_swarm-0.2.2/agency_swarm/agency/genesis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.124850 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/AgentCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.124850 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.124850 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisAgency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.124850 agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.124850 agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.128850 agency_swarm-0.2.2/agency_swarm/agency/genesis/OpenAPICreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/OpenAPICreator/OpenAPICreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/OpenAPICreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/OpenAPICreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.128850 agency_swarm-0.2.2/agency_swarm/agency/genesis/OpenAPICreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.128850 agency_swarm-0.2.2/agency_swarm/agency/genesis/ToolCreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/ToolCreator/ToolCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/ToolCreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/ToolCreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.128850 agency_swarm-0.2.2/agency_swarm/agency/genesis/ToolCreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/manifesto.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agency/genesis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.128850 agency_swarm-0.2.2/agency_swarm/agents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.128850 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/instructions.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.132850 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/GoBack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/Scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.132850 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/util/get_b64_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.132850 agency_swarm-0.2.2/agency_swarm/agents/Devid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/Devid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.132850 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/ChangeFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/CheckCurrentDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/CommandExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/DirectoryNavigator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/FileMover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/FileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/FileWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/ListDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.136850 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/util/format_file_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30706 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/agents/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.136850 agency_swarm-0.2.2/agency_swarm/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/messages/message_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.136850 agency_swarm-0.2.2/agency_swarm/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/threads/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/threads/thread_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.136850 agency_swarm-0.2.2/agency_swarm/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/tools/BaseTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/tools/ToolFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.136850 agency_swarm-0.2.2/agency_swarm/tools/oai/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/tools/oai/CodeInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/tools/oai/FileSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/tools/oai/Retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/tools/oai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.136850 agency_swarm-0.2.2/agency_swarm/user/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/user/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.136850 agency_swarm-0.2.2/agency_swarm/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.140850 agency_swarm-0.2.2/agency_swarm/util/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/cli/create_agent_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/cli/import_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.140850 agency_swarm-0.2.2/agency_swarm/util/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/helpers/get_available_agent_descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/helpers/list_available_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/oai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/agency_swarm/util/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.148850 agency_swarm-0.2.2/agency_swarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-05-09 05:41:22.000000 agency_swarm-0.2.2/agency_swarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-09 05:41:22.000000 agency_swarm-0.2.2/agency_swarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:41:22.000000 agency_swarm-0.2.2/agency_swarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 05:41:22.000000 agency_swarm-0.2.2/agency_swarm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 05:41:22.000000 agency_swarm-0.2.2/agency_swarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 05:41:22.000000 agency_swarm-0.2.2/agency_swarm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.140850 agency_swarm-0.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.140850 agency_swarm-0.2.2/docs/advanced-usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/advanced-usage/agencies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/advanced-usage/agents.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/advanced-usage/azure-openai.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/advanced-usage/open-source-models.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/advanced-usage/tools.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.140850 agency_swarm-0.2.2/docs/introduction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/introduction/showcase.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/docs/quick_start.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.144850 agency_swarm-0.2.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    49298 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/notebooks/Agency_Swarm_with_Open_Source_Model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/notebooks/agency_async.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/notebooks/azure.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/notebooks/genesis_agency.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/notebooks/web_browser_agent.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:41:22.148850 agency_swarm-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.144850 agency_swarm-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.116850 agency_swarm-0.2.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.144850 agency_swarm-0.2.2/tests/data/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/files/csv-test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   102408 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/files/generated_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/files/test-docx.docx
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/files/test-html.html
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/files/test-md.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/files/test-pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/files/test-txt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/files/test-xml.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.144850 agency_swarm-0.2.2/tests/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/schemas/ga4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/schemas/get-headers-params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/schemas/get-weather.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/schemas/relevance.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.144850 agency_swarm-0.2.2/tests/data/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/data/tools/ExampleTool1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:41:22.148850 agency_swarm-0.2.2/tests/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/demos/demo_gradio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/demos/streaming_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/demos/term_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/test_agency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-09 05:41:18.000000 agency_swarm-0.2.2/tests/test_tool_factory.py
```

### Comparing `agency_swarm-0.2.1/.github/workflows/close-issues.yml` & `agency_swarm-0.2.2/.github/workflows/close-issues.yml`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/.github/workflows/docs.yml` & `agency_swarm-0.2.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/.github/workflows/publish.yml` & `agency_swarm-0.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/.github/workflows/test.yml` & `agency_swarm-0.2.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/.gitignore` & `agency_swarm-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/CONTRIBUTING.md` & `agency_swarm-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/LICENSE` & `agency_swarm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/PKG-INFO` & `agency_swarm-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agency-swarm
-Version: 0.2.1
+Version: 0.2.2
 Summary: An open source agent orchestration framework built on top of the latest OpenAI Assistants API.
 Home-page: https://github.com/VRSEN/agency-swarm
 Author: VRSEN
 Author-email: VRSEN <arseny9795@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Arsenii Shatokhin
@@ -30,16 +30,16 @@
 Project-URL: homepage, https://github.com/VRSEN/agency-swarm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.23.3
-Requires-Dist: instructor==1.2.2
+Requires-Dist: openai==1.27.0
+Requires-Dist: instructor==1.2.6
 Requires-Dist: deepdiff==6.7.1
 Requires-Dist: termcolor==2.3.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: rich==13.7.0
 Requires-Dist: jsonref==1.1.0
 
 # 🐝 Agency Swarm
```

### Comparing `agency_swarm-0.2.1/README.md` & `agency_swarm-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/agency.py` & `agency_swarm-0.2.2/agency_swarm/agency/agency.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,22 +129,33 @@
             attachments (List[dict], optional): A list of attachments to be sent with the message, following openai format. Defaults to None.
             tool_choice (dict, optional): The tool choice for the recipient agent to use. Defaults to None.
 
         Returns:
             Generator or final response: Depending on the 'yield_messages' flag, this method returns either a generator yielding intermediate messages or the final response from the main thread.
         """
         if yield_messages:
-            print("Warning: yield_messages parameter is deprecated. Use streaming instead.")
+            print("Warning: yield_messages parameter will be deprecated soon. Use streaming instead.")
 
-        return self.main_thread.get_completion(message=message,
+        res = self.main_thread.get_completion(message=message,
                                                message_files=message_files,
                                                attachments=attachments,
                                                recipient_agent=recipient_agent,
                                                additional_instructions=additional_instructions,
-                                               tool_choice=tool_choice)
+                                               tool_choice=tool_choice,
+                                               yield_messages=yield_messages)
+
+        if not yield_messages:
+            while True:
+                try:
+                    next(res)
+                except StopIteration as e:
+                    return e.value
+
+        return res
+
 
     def get_completion_stream(self,
                               message: str,
                               event_handler: type(AgencyEventHandler),
                               message_files: List[str] = None,
                               recipient_agent: Agent = None,
                               additional_instructions: str = None,
@@ -162,32 +173,32 @@
             additional_instructions (str, optional): Additional instructions to be sent with the message. Defaults to None.
             attachments (List[dict], optional): A list of attachments to be sent with the message, following openai format. Defaults to None.
             tool_choice (dict, optional): The tool choice for the recipient agent to use. Defaults to None.
 
         Returns:
             Final response: Final response from the main thread.
         """
-        if self.async_mode:
-            raise Exception("Streaming is not supported in async mode.")
-
         if not inspect.isclass(event_handler):
             raise Exception("Event handler must not be an instance.")
 
         res = self.main_thread.get_completion_stream(message=message,
                                                       message_files=message_files,
                                                       event_handler=event_handler,
                                                       attachments=attachments,
                                                       recipient_agent=recipient_agent,
                                                       additional_instructions=additional_instructions,
                                                       tool_choice=tool_choice
                                                       )
 
-        event_handler.on_all_streams_end()
-
-        return res
+        while True:
+            try:
+                next(res)
+            except StopIteration as e:
+                event_handler.on_all_streams_end()
+                return e.value
 
     def demo_gradio(self, height=450, dark_mode=True, **kwargs):
         """
         Launches a Gradio-based demo interface for the agency chatbot.
 
         Parameters:
             height (int, optional): The height of the chatbot widget in the Gradio interface. Default is 600.
@@ -348,15 +359,15 @@
 
                             chatbot_queue.put(self.message_output.get_formatted_header() + "\n")
                             chatbot_queue.put(tool_call.function.output)
 
                 @override
                 @classmethod
                 def on_all_streams_end(cls):
-                    self.message_output = None
+                    cls.message_output = None
                     chatbot_queue.put("[end]")
 
             def bot(original_message, history):
                 nonlocal message_file_ids
                 nonlocal message_file_names
                 nonlocal recipient_agent
                 print("Message files: ", message_file_ids)
```

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/instructions.md` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,27 +67,26 @@
                               self.agent_description,
                               instructions=self.instructions,
                               code_interpreter=True if "CodeInterpreter" in self.default_tools else None,
                               include_example_tool=False)
 
         # # create or append to init file
         path = self.shared_state.get("agency_path")
-        folder_name = self.agent_name.lower().replace(" ", "_")
         class_name = self.agent_name.replace(" ", "").strip()
         if not os.path.isfile("__init__.py"):
             with open("__init__.py", "w") as f:
-                f.write(f"from .{folder_name} import {class_name}")
+                f.write(f"from .{class_name} import {class_name}")
         else:
             with open("__init__.py", "a") as f:
-                f.write(f"\nfrom .{folder_name} import {class_name}")
+                f.write(f"\nfrom .{class_name} import {class_name}")
 
         # add agent on second line to agency.py
         with open("agency.py", "r") as f:
             lines = f.readlines()
-            lines.insert(1, f"from {self.agent_name} import {self.agent_name}\n")
+            lines.insert(1, f"from {class_name} import {class_name}\n")
 
         with open("agency.py", "w") as f:
             f.writelines(lines)
 
         os.chdir(self.shared_state.get("default_folder"))
 
         if "ceo" in self.agent_name.lower():
```

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisAgency.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisAgency.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/instructions.md` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/OpenAPICreator/instructions.md` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/OpenAPICreator/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/ToolCreator/instructions.md` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/ToolCreator/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         value = self.shared_state.get("key")
         
         return "Result of AnotherTool operation"
 ```
 
 This is useful to pass information between tools or agents or to verify the state of the system.  
 
-Remember, you must output the resulting python tool code as a whole, so the user can just copy and paste it into his program. Each tool code snippet must be ready to use. It must not contain any placeholders or hypothetical examples."""
+Remember, you must output the resulting python tool code as a whole in a code block, so the user can just copy and paste it into his program. Each tool code snippet must be ready to use. It must not contain any placeholders or hypothetical examples."""
 
 history = [
             {
                 "role": "system",
                 "content": prompt
             },
         ]
@@ -157,22 +157,23 @@
         history.append({
                 "role": "user",
                 "content": message
             })
 
         messages = history.copy()
 
-        # use the last 5 messages
-        messages = messages[-5:]
+        # use the last 6 messages
+        messages = messages[-6:]
 
         # add system message upfront
         messages.insert(0, history[0])
 
         n = 0
-        error_message = ""
+        code = ""
+        content = ""
         while n < 3:
             resp = client.chat.completions.create(
                 messages=messages,
                 model="gpt-4-turbo",
                 temperature=0,
             )
 
@@ -191,42 +192,30 @@
                 code = match[-1].strip()
                 history.append(
                     {
                         "role": "assistant",
                         "content": content
                     }
                 )
-
                 break
             else:
                 messages.append(
                     {
                         "role": "user",
-                        "content": f"Error: Could not find the code block in the response. Please try again."
+                        "content": f"Error: Could not find the python code block in the response. Please try again."
                     }
                 )
 
             n += 1
 
         if n == 3 or not code:
-            history.append(
-                {
-                    "role": "assistant",
-                    "content": content
-                }
-            )
-            history.append(
-                {
-                    "role": "user",
-                    "content": error_message
-                }
-            )
+            # remove last message from history
+            history.pop()
             os.chdir(self.shared_state.get("default_folder"))
-            return "Error: Could not generate a valid file: " + error_message
-
+            return "Error: Could not generate a valid file."
         try:
             with open("./tools/" + self.tool_name + ".py", "w") as file:
                 file.write(code)
 
             os.chdir(self.shared_state.get("default_folder"))
             return f'{content}\n\nPlease make sure to now test this tool if possible.'
         except Exception as e:
```

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/manifesto.md` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/manifesto.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agency/genesis/util.py` & `agency_swarm-0.2.2/agency_swarm/agency/genesis/util.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/instructions.md` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/Scroll.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/Scroll.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py` & `agency_swarm-0.2.2/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/Devid/Devid.py` & `agency_swarm-0.2.2/agency_swarm/agents/Devid/Devid.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/Devid/instructions.md` & `agency_swarm-0.2.2/agency_swarm/agents/Devid/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/ChangeFile.py` & `agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/ChangeFile.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/CommandExecutor.py` & `agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/CommandExecutor.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/DirectoryNavigator.py` & `agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/DirectoryNavigator.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/FileMover.py` & `agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/FileMover.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/FileReader.py` & `agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/FileReader.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/FileWriter.py` & `agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/FileWriter.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/ListDir.py` & `agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/ListDir.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/Devid/tools/util/format_file_deps.py` & `agency_swarm-0.2.2/agency_swarm/agents/Devid/tools/util/format_file_deps.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/agents/agent.py` & `agency_swarm-0.2.2/agency_swarm/agents/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             name: str = None,
             description: str = None,
             instructions: str = "",
             tools: List[Union[Type[BaseTool], Type[FileSearch], Type[CodeInterpreter], type[Retrieval]]] = None,
             tool_resources: ToolResources = None,
             temperature: float = None,
             top_p: float = None,
-            response_format: str | dict = "auto",
+            response_format: Union[str, dict] = "auto",
             tools_folder: str = None,
             files_folder: Union[List[str], str] = None,
             schemas_folder: Union[List[str], str] = None,
             api_headers: Dict[str, Dict[str, str]] = None,
             api_params: Dict[str, Dict[str, str]] = None,
             file_ids: List[str] = None,
             metadata: Dict[str, str] = None,
@@ -614,17 +614,20 @@
         elif "./instructions.md" in self.instructions or "./instructions.txt" in self.instructions:
             raise Exception("Instructions file not found.")
 
     def get_class_folder_path(self):
         try:
             # First, try to use the __file__ attribute of the module
             return os.path.abspath(os.path.dirname(self.__module__.__file__))
-        except AttributeError:
+        except (TypeError, OSError, AttributeError) as e:
             # If that fails, fall back to inspect
-            class_file = inspect.getfile(self.__class__)
+            try:
+                class_file = inspect.getfile(self.__class__)
+            except (TypeError, OSError, AttributeError) as e:
+                return "./"
             return os.path.abspath(os.path.realpath(os.path.dirname(class_file)))
 
     def add_shared_instructions(self, instructions: str):
         if not instructions:
             return
 
         if self._shared_instructions is None:
```

### Comparing `agency_swarm-0.2.1/agency_swarm/cli.py` & `agency_swarm-0.2.2/agency_swarm/cli.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/messages/message_output.py` & `agency_swarm-0.2.2/agency_swarm/messages/message_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Literal
 import hashlib
 from rich.markdown import Markdown
 from rich.console import Console, Group
 from rich.live import Live
 
 console = Console()
-live_display = Live()
 
 class MessageOutput:
     def __init__(self, msg_type: Literal["function", "function_output", "text", "system"], sender_name: str,
                  receiver_name: str, content):
         self.msg_type = msg_type
         self.sender_name = str(sender_name)
         self.receiver_name = str(receiver_name)
@@ -106,16 +105,17 @@
         # Initialize Live display if not already done
         self.live_display = Live(vertical_overflow="visible")
         self.live_display.start()
 
         console.rule()
 
     def __del__(self):
-        self.live_display.stop()
-        self.live_display = None
+        if self.live_display:
+            self.live_display.stop()
+            self.live_display = None
 
     def cprint_update(self, snapshot):
         """
         Update the display with new snapshot content.
         """
         self.content = snapshot  # Update content with the latest snapshot
```

### Comparing `agency_swarm-0.2.1/agency_swarm/threads/thread.py` & `agency_swarm-0.2.2/agency_swarm/threads/thread.py`

 * *Files 16% similar despite different names*

```diff
@@ -70,32 +70,35 @@
                        tool_choice: AssistantToolChoice = None,
                        yield_messages: bool = False
                        ):
         if yield_messages:
             # warn that it is deprecated
             print("Warning: yield_messages is deprecated. Use get_completion_stream instead.")
 
+        if not recipient_agent:
+            recipient_agent = self.recipient_agent
+
+        if not attachments:
+            attachments = []
+
         if message_files:
             recipient_tools = []
 
-            if FileSearch in self.recipient_agent.tools:
+            if FileSearch in recipient_agent.tools:
                 recipient_tools.append({"type": "file_search"})
-            if CodeInterpreter in self.recipient_agent.tools:
+            if CodeInterpreter in recipient_agent.tools:
                 recipient_tools.append({"type": "code_interpreter"})
 
             for file_id in message_files:
                 attachments.append({"file_id": file_id,
                                     "tools": recipient_tools or [{"type": "file_search"}]})
 
         if not self.thread:
             self.init_thread()
 
-        if not recipient_agent:
-            recipient_agent = self.recipient_agent
-
         if event_handler:
             event_handler.agent_name = self.agent.name
             event_handler.recipient_agent_name = recipient_agent.name
 
         # Determine the sender's name based on the agent type
         sender_name = "user" if isinstance(self.agent, User) else self.agent.name
         playground_url = f'https://platform.openai.com/playground?assistant={recipient_agent.assistant.id}&mode=assistant&thread={self.thread.id}'
@@ -105,35 +108,48 @@
         self.client.beta.threads.messages.create(
             thread_id=self.thread.id,
             role="user",
             content=message,
             attachments=attachments
         )
 
+        if yield_messages:
+            yield MessageOutput("text", self.agent.name, recipient_agent.name, message)
+
         self._create_run(recipient_agent, additional_instructions, event_handler, tool_choice)
 
         error_attempts = 0
         validation_attempts = 0
         full_message = ""
         while True:
             self._run_until_done()
 
             # function execution
             if self.run.status == "requires_action":
                 tool_calls = self.run.required_action.submit_tool_outputs.tool_calls
                 tool_outputs = []
                 tool_names = []
                 for tool_call in tool_calls:
+                    if yield_messages:
+                        yield MessageOutput("function", recipient_agent.name, self.agent.name,
+                                            str(tool_call.function))
+
                     output = self.execute_tool(tool_call, recipient_agent, event_handler, tool_names)
                     if inspect.isgenerator(output):
                         try:
                             while True:
                                 item = next(output)
+                                if isinstance(item, MessageOutput) and yield_messages:
+                                    yield item
                         except StopIteration as e:
                             output = e.value
+                    else:
+                        if yield_messages:
+                            yield MessageOutput("function_output", tool_call.function.name, recipient_agent.name,
+                                                output)
                     if event_handler:
                         event_handler.agent_name = self.agent.name
                         event_handler.recipient_agent_name = recipient_agent.name
 
                     tool_outputs.append({"tool_call_id": tool_call.id, "output": str(output)})
                     tool_names.append(tool_call.function.name)
 
@@ -141,28 +157,39 @@
                 try:
                     self._submit_tool_outputs(tool_outputs, event_handler)
                 except BadRequestError as e:
                     if 'Runs in status "expired"' in e.message:
                         self.client.beta.threads.messages.create(
                             thread_id=self.thread.id,
                             role="user",
-                            content="Please repeat the exact same function calls again in the same order."
+                            content="Please repeat the exact same tool calls in the same order with the same arguments."
                         )
 
-                        self._create_run(recipient_agent, additional_instructions, event_handler, tool_choice)
+                        self._create_run(recipient_agent, additional_instructions, event_handler, 'required',
+                                         temperature=0)
 
                         self._run_until_done()
 
                         if self.run.status != "requires_action":
                             raise Exception("Run Failed. Error: ", self.run.last_error)
 
                         # change tool call ids
                         tool_calls = self.run.required_action.submit_tool_outputs.tool_calls
-                        for i, tool_call in enumerate(tool_calls):
-                            tool_outputs[i]["tool_call_id"] = tool_call.id
+
+                        if len(tool_calls) != len(tool_outputs):
+                            tool_outputs = []
+                            for i, tool_call in enumerate(tool_calls):
+                                tool_outputs.append({"tool_call_id": tool_call.id,
+                                                     "output": "Error: openai run timed out. You can try again one more time."})
+                        else:
+                            for i, tool_name in enumerate(tool_names):
+                                for tool_call in tool_calls:
+                                    if tool_call.function.name == tool_name:
+                                        tool_outputs[i]["tool_call_id"] = tool_call.id
+                                        break
 
                         self._submit_tool_outputs(tool_outputs, event_handler)
                     else:
                         raise e
             # error
             elif self.run.status == "failed":
                 full_message += self._get_last_message_text() + "\n"
@@ -181,62 +208,71 @@
                     error_attempts += 1
                 else:
                     raise Exception("OpenAI Run Failed. Error: ", self.run.last_error.message)
             # return assistant message
             else:
                 full_message += self._get_last_message_text()
 
+                if yield_messages:
+                    yield MessageOutput("text", recipient_agent.name, self.agent.name, full_message)
+
                 if recipient_agent.response_validator:
                     try:
                         if isinstance(recipient_agent, Agent):
                             recipient_agent.response_validator(message=full_message)
                     except Exception as e:
                         if validation_attempts < recipient_agent.validation_attempts:
                             message = self.client.beta.threads.messages.create(
                                 thread_id=self.thread.id,
                                 role="user",
                                 content=str(e),
                             )
 
+                            if yield_messages:
+                                yield MessageOutput("text", self.agent.name, recipient_agent.name,
+                                                    message.content[0].text.value)
+
                             if event_handler:
                                 handler = event_handler()
                                 handler.on_message_created(message)
                                 handler.on_message_done(message)
 
                             validation_attempts += 1
 
                             self._create_run(recipient_agent, additional_instructions, event_handler, tool_choice)
 
                             continue
 
                 return full_message
 
-    def _create_run(self, recipient_agent, additional_instructions, event_handler, tool_choice):
+    def _create_run(self, recipient_agent, additional_instructions, event_handler, tool_choice, temperature=None):
         if event_handler:
             with self.client.beta.threads.runs.stream(
                     thread_id=self.thread.id,
                     event_handler=event_handler(),
                     assistant_id=recipient_agent.id,
                     additional_instructions=additional_instructions,
                     tool_choice=tool_choice,
                     max_prompt_tokens=recipient_agent.max_prompt_tokens,
                     max_completion_tokens=recipient_agent.max_completion_tokens,
                     truncation_strategy=recipient_agent.truncation_strategy,
+                    temperature=temperature
             ) as stream:
                 stream.until_done()
                 self.run = stream.get_final_run()
         else:
             self.run = self.client.beta.threads.runs.create_and_poll(
                 thread_id=self.thread.id,
                 assistant_id=recipient_agent.id,
                 additional_instructions=additional_instructions,
                 tool_choice=tool_choice,
                 max_prompt_tokens=recipient_agent.max_prompt_tokens,
                 max_completion_tokens=recipient_agent.max_completion_tokens,
                 truncation_strategy=recipient_agent.truncation_strategy,
+                temperature=temperature
             )
 
     def _run_until_done(self):
         while self.run.status in ['queued', 'in_progress', "cancelling"]:
             time.sleep(0.5)
             self.run = self.client.beta.threads.runs.retrieve(
                 thread_id=self.thread.id,
```

### Comparing `agency_swarm-0.2.1/agency_swarm/threads/thread_async.py` & `agency_swarm-0.2.2/agency_swarm/threads/thread_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,27 @@
                message: str,
                message_files: List[str] = None,
                attachments: Optional[List[dict]] = None,
                recipient_agent=None,
                additional_instructions: str = None,
                tool_choice: AssistantToolChoice = None
                ):
-        output = super().get_completion(message=message,
+        gen = super().get_completion(message=message,
                                         message_files=message_files,
                                         attachments=attachments,
                                         recipient_agent=recipient_agent,
                                         additional_instructions=additional_instructions,
                                         tool_choice=tool_choice)
 
-        self.response = f"""{self.recipient_agent.name}'s Response: '{output}'"""
+        while True:
+            try:
+                next(gen)
+            except StopIteration as e:
+                self.response = f"""{self.recipient_agent.name}'s Response: '{e.value}'"""
+                break
 
         return
 
     def get_completion_async(self,
                              message: str,
                              message_files: List[str] = None,
                              attachments: Optional[List[dict]] = None,
```

### Comparing `agency_swarm-0.2.1/agency_swarm/tools/BaseTool.py` & `agency_swarm-0.2.2/agency_swarm/tools/BaseTool.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/tools/ToolFactory.py` & `agency_swarm-0.2.2/agency_swarm/tools/ToolFactory.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/util/cli/create_agent_template.py` & `agency_swarm-0.2.2/agency_swarm/util/cli/create_agent_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,35 +10,34 @@
                           include_example_tool=True):
     if not agent_name:
         agent_name = input("Enter agent name: ")
     if not agent_description:
         agent_description = input("Enter agent description: ")
 
     class_name = agent_name.replace(" ", "").strip()
-    folder_name = agent_name  # .lower().replace(" ", "_").strip()
 
     # create folder
-    path = os.path.join(path, folder_name) + "/"
+    path = os.path.join(path, class_name) + "/"
     if os.path.isdir(path):
         raise Exception("Folder already exists.")
     os.mkdir(path)
 
     # create agent file
-    with open(path + folder_name + ".py", "w") as f:
+    with open(path + class_name + ".py", "w") as f:
         f.write(agent_template.format(
             class_name=class_name,
             agent_name=agent_name,
             agent_description=agent_description,
             ext="md" if not use_txt else "txt",
             code_interpreter="CodeInterpreter" if code_interpreter else "",
             code_interpreter_import="from agency_swarm.tools import CodeInterpreter" if code_interpreter else ""
         ))
 
     with open(path + "__init__.py", "w") as f:
-        f.write(f"from .{folder_name} import {class_name}")
+        f.write(f"from .{class_name} import {class_name}")
 
     # create instructions file
     instructions_path = "instructions.md" if not use_txt else "instructions.txt"
     with open(path + instructions_path, "w") as f:
         if instructions:
             f.write(instructions)
         else:
@@ -53,15 +52,15 @@
     #     f.write("")
 
     if include_example_tool:
         with open(path + "tools/" + "ExampleTool.py", "w") as f:
             f.write(example_tool_template)
 
     print("Agent folder created successfully.")
-    print(f"Import it with: from {folder_name} import {class_name}")
+    print(f"Import it with: from {class_name} import {class_name}")
 
 
 agent_template = """from agency_swarm.agents import Agent
 {code_interpreter_import}
 
 class {class_name}(Agent):
     def __init__(self):
```

### Comparing `agency_swarm-0.2.1/agency_swarm/util/cli/import_agent.py` & `agency_swarm-0.2.2/agency_swarm/util/cli/import_agent.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/util/event_handler.py` & `agency_swarm-0.2.2/agency_swarm/util/event_handler.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/util/helpers/get_available_agent_descriptions.py` & `agency_swarm-0.2.2/agency_swarm/util/helpers/get_available_agent_descriptions.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/util/helpers/list_available_agents.py` & `agency_swarm-0.2.2/agency_swarm/util/helpers/list_available_agents.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/util/oai.py` & `agency_swarm-0.2.2/agency_swarm/util/oai.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/util/openapi.py` & `agency_swarm-0.2.2/agency_swarm/util/openapi.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm/util/schema.py` & `agency_swarm-0.2.2/agency_swarm/util/schema.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/agency_swarm.egg-info/PKG-INFO` & `agency_swarm-0.2.2/agency_swarm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agency-swarm
-Version: 0.2.1
+Version: 0.2.2
 Summary: An open source agent orchestration framework built on top of the latest OpenAI Assistants API.
 Home-page: https://github.com/VRSEN/agency-swarm
 Author: VRSEN
 Author-email: VRSEN <arseny9795@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Arsenii Shatokhin
@@ -30,16 +30,16 @@
 Project-URL: homepage, https://github.com/VRSEN/agency-swarm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.23.3
-Requires-Dist: instructor==1.2.2
+Requires-Dist: openai==1.27.0
+Requires-Dist: instructor==1.2.6
 Requires-Dist: deepdiff==6.7.1
 Requires-Dist: termcolor==2.3.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: rich==13.7.0
 Requires-Dist: jsonref==1.1.0
 
 # 🐝 Agency Swarm
```

### Comparing `agency_swarm-0.2.1/agency_swarm.egg-info/SOURCES.txt` & `agency_swarm-0.2.2/agency_swarm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 docs/deployment.md
 docs/examples.md
 docs/index.md
 docs/quick_start.md
 docs/advanced-usage/agencies.md
 docs/advanced-usage/agents.md
 docs/advanced-usage/azure-openai.md
+docs/advanced-usage/open-source-models.md
 docs/advanced-usage/tools.md
 docs/introduction/showcase.md
 notebooks/Agency_Swarm_with_Open_Source_Model.ipynb
 notebooks/agency_async.ipynb
 notebooks/azure.ipynb
 notebooks/genesis_agency.ipynb
 notebooks/web_browser_agent.ipynb
```

### Comparing `agency_swarm-0.2.1/docs/advanced-usage/agencies.md` & `agency_swarm-0.2.2/docs/advanced-usage/agencies.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/docs/advanced-usage/agents.md` & `agency_swarm-0.2.2/docs/advanced-usage/agents.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/docs/advanced-usage/azure-openai.md` & `agency_swarm-0.2.2/docs/advanced-usage/azure-openai.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/docs/advanced-usage/tools.md` & `agency_swarm-0.2.2/docs/advanced-usage/tools.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/docs/contributing.md` & `agency_swarm-0.2.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/docs/deployment.md` & `agency_swarm-0.2.2/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/docs/examples.md` & `agency_swarm-0.2.2/docs/examples.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/docs/index.md` & `agency_swarm-0.2.2/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,19 @@
 
 1. **Does not write prompts** for you.
 2. Prevents hallucinations with automatic **type checking and error correction** with [instructor](https://github.com/jxnl/instructor/tree/main)
 3. Allows you to easily define **communication flows**.
 
 ### **AutoGen** vs Agency Swarm
 
-In AutoGen, the next speaker is determined with an extra call to the model that emulates "role play" between the agents. [[1]](https://microsoft.github.https://microsoft.github.io/autogen/blog/2023/12/29/AgentDescriptionsio/autogen/blog/2023/12/29/AgentDescriptions) Not only this is very inefficient, but it also makes the system less controllable and less customizable, because you cannot control which agent can communicate with which other agent. In Agency Swarm, on the other hand, the communication is handled through the special `SendMessage` tool. [[2]](https://github.com/VRSEN/agency-swarm/blob/81ff3ad5d854729bcfa755f19480d681efa8e72b/agency_swarm/agency/agency.py#L528) Your agents will determine who to communicate with based on their own descriptions. The caller agent will the receive the response as the function output, which makes it a lot more natural for your agents to understand the communication flow.
+In AutoGen, by default, the next speaker is determined with an extra call to the model that emulates "role play" between the agents. [[1]](https://microsoft.github.https://microsoft.github.io/autogen/blog/2023/12/29/AgentDescriptionsio/autogen/blog/2023/12/29/AgentDescriptions) Not only this is very inefficient, but it also makes the system less controllable and less customizable, because you cannot control which agent can communicate with which other agent. 
+
+Recently, autogen has added support for [determining the next speaker based on certain hardcoded conditions](https://microsoft.github.io/autogen/docs/notebooks/agentchat_groupchat_customized/). While this does make your system more customizable, it completely undermines the main benefit of agentic systems - adaptability. In my opinion, **you should only determine the boundaries for your agents, not the conditions themselves, as you are unlikely to account for every single condition in the real world.** ([#113](https://github.com/VRSEN/agency-swarm/issues/113))
+
+In Agency Swarm, on the other hand, the communication is handled through the special `SendMessage` tool. [[2]](https://github.com/VRSEN/agency-swarm/blob/81ff3ad5d854729bcfa755f19480d681efa8e72b/agency_swarm/agency/agency.py#L528) Your agents will determine who to communicate with by themselves based on their own descriptions. All you have to do is set the boundaries for their communication inside the agency chart.
 
 ### **CrewAI** vs Agency Swarm
 
 CrewAI introduces a concept of "process" [[3]](https://docs.crewai.com/core-concepts/Processes/) into agent communication, which provides some control over the communication flow. However, the biggest problem with CrewAI is that it is built on top of Langchain, which was created long before any function-calling models were released. This means that there is no type checking or error correction, so any action that your agent takes (which is the most important part of the system) could cause the whole system to go down if the model hallucinates. The sole advantage of CrewAI is its compatibility with open-source models.
 
 ## Need help?
```

### Comparing `agency_swarm-0.2.1/docs/quick_start.md` & `agency_swarm-0.2.2/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/mkdocs.yml` & `agency_swarm-0.2.2/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     - content.code.select
     - content.code.copy
   name: material
   palette:
     # Palette toggle for light mode
     - media: "(prefers-color-scheme: light)"
       scheme: default
-      primary: black
+      primary: amber
+      accent: yellow
       toggle:
         icon: material/brightness-7
         name: Switch to dark mode
     # Palette toggle for dark mode
     - media: "(prefers-color-scheme: dark)"
       scheme: slate
       primary: amber
@@ -42,14 +43,15 @@
   - Quick Start: "quick_start.md"
   - Advanced Usage:
     - Advanced Tools: "advanced-usage/tools.md"
     - Agents: "advanced-usage/agents.md"
     - Agencies: "advanced-usage/agencies.md"
     - Azure OpenAI: "advanced-usage/azure-openai.md"
   - Deployment to Production: "deployment.md"
+  - Open Source Models: "advanced-usage/open-source-models.md"
   - API Reference: "api.md"
   - Contributing: "contributing.md"
   - Examples: "examples.md"
 plugins:
   - mkdocs-jupyter:
       ignore_h1_titles: true
       execute: false
@@ -64,12 +66,12 @@
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
 extra:
   generator: false
   social:
     - icon: fontawesome/brands/mastodon
-      link: https://www.vrsen.ai/
+      link: https://agents.vrsen.ai/
     - icon: fontawesome/brands/github
       link: https://github.com/VRSEN/agency-swarm
     - icon: fontawesome/brands/x-twitter
       link: https://twitter.com/__vrsen__
```

### Comparing `agency_swarm-0.2.1/notebooks/Agency_Swarm_with_Open_Source_Model.ipynb` & `agency_swarm-0.2.2/notebooks/Agency_Swarm_with_Open_Source_Model.ipynb`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/notebooks/agency_async.ipynb` & `agency_swarm-0.2.2/notebooks/agency_async.ipynb`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/notebooks/azure.ipynb` & `agency_swarm-0.2.2/notebooks/azure.ipynb`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/notebooks/genesis_agency.ipynb` & `agency_swarm-0.2.2/notebooks/genesis_agency.ipynb`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/notebooks/web_browser_agent.ipynb` & `agency_swarm-0.2.2/notebooks/web_browser_agent.ipynb`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/pyproject.toml` & `agency_swarm-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-    "openai==1.23.3",
-    "instructor==1.2.2",
+    "openai==1.27.0",
+    "instructor==1.2.6",
     "deepdiff==6.7.1",
     "termcolor==2.3.0",
     "python-dotenv==1.0.0",
     "rich==13.7.0",
     "jsonref==1.1.0"
 ]
 requires-python = ">=3.7"
```

### Comparing `agency_swarm-0.2.1/run_tests.py` & `agency_swarm-0.2.2/run_tests.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/setup.py` & `agency_swarm-0.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='agency-swarm',
-    version='0.2.1',
+    version='0.2.2',
     author='VRSEN',
     author_email='arseny9795@gmail.com',
     description='An opensource agent orchestration framework built on top of the latest OpenAI Assistants API.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VRSEN/agency-swarm',
     packages=find_packages(exclude=['tests', 'tests.*']),
```

### Comparing `agency_swarm-0.2.1/tests/data/files/csv-test.csv` & `agency_swarm-0.2.2/tests/data/files/csv-test.csv`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/data/files/generated_data.json` & `agency_swarm-0.2.2/tests/data/files/generated_data.json`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/data/files/test-docx.docx` & `agency_swarm-0.2.2/tests/data/files/test-docx.docx`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/data/files/test-html.html` & `agency_swarm-0.2.2/tests/data/files/test-html.html`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/data/files/test-pdf.pdf` & `agency_swarm-0.2.2/tests/data/files/test-pdf.pdf`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/data/schemas/ga4.json` & `agency_swarm-0.2.2/tests/data/schemas/ga4.json`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/data/schemas/get-headers-params.json` & `agency_swarm-0.2.2/tests/data/schemas/get-headers-params.json`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/data/schemas/get-weather.json` & `agency_swarm-0.2.2/tests/data/schemas/get-weather.json`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/data/schemas/relevance.json` & `agency_swarm-0.2.2/tests/data/schemas/relevance.json`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/demos/demo_gradio.py` & `agency_swarm-0.2.2/tests/demos/demo_gradio.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/demos/streaming_demo.py` & `agency_swarm-0.2.2/tests/demos/streaming_demo.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/demos/term_demo.py` & `agency_swarm-0.2.2/tests/demos/term_demo.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.1/tests/test_agency.py` & `agency_swarm-0.2.2/tests/test_agency.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import os
 import shutil
 import sys
 import time
 import unittest
 
+from openai.types.beta.threads import Text
 from openai.types.beta.threads.runs import ToolCall
 
 from agency_swarm.tools import CodeInterpreter, FileSearch
 
 sys.path.insert(0, '../agency-swarm')
 from agency_swarm.util import create_agent_template
 
@@ -383,18 +384,44 @@
         print("TestAgent1 tools", self.__class__.agent1.tools)
         self.__class__.agency.get_completion("Please tell TestAgent2 hello.",
                                              tool_choice={"type": "function", "function": {"name": "SendMessage"}},
                                              recipient_agent=self.__class__.agent1)
 
         time.sleep(10)
 
-        message = self.__class__.agency.get_completion(
+        num_on_all_streams_end_calls = 0
+        delta_value = ""
+        full_text = ""
+
+        class EventHandler(AgencyEventHandler):
+            @override
+            def on_text_delta(self, delta, snapshot):
+                nonlocal delta_value
+                delta_value += delta.value
+
+            @override
+            def on_text_done(self, text: Text) -> None:
+                nonlocal full_text
+                full_text += text.value
+
+            @override
+            @classmethod
+            def on_all_streams_end(cls):
+                nonlocal num_on_all_streams_end_calls
+                num_on_all_streams_end_calls += 1
+
+        message = self.__class__.agency.get_completion_stream(
             "Please check response. If output includes `TestAgent2's Response`, say 'success'. If the function output does not include `TestAgent2's Response`, or if you get a System Notification, or an error instead, say 'error'.",
             tool_choice={"type": "function", "function": {"name": "GetResponse"}},
-            recipient_agent=self.__class__.agent1)
+            recipient_agent=self.__class__.agent1,
+            event_handler=EventHandler)
+
+        self.assertTrue(num_on_all_streams_end_calls == 1)
+
+        self.assertTrue(delta_value == full_text == message)
 
         if 'error' in message.lower():
             print(self.__class__.agency.get_completion("Explain why you said error."))
             self.assertFalse('error' in message.lower())
 
         for agent_name, threads in self.__class__.agency.agents_and_threads.items():
             for other_agent_name, thread in threads.items():
```

### Comparing `agency_swarm-0.2.1/tests/test_tool_factory.py` & `agency_swarm-0.2.2/tests/test_tool_factory.py`

 * *Files identical despite different names*

