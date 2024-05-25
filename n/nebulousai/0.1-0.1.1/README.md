# Comparing `tmp/nebulousai-0.1.tar.gz` & `tmp/nebulousai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nebulousai-0.1.tar", last modified: Sun May 19 12:03:34 2024, max compression
+gzip compressed data, was "nebulousai-0.1.1.tar", last modified: Sat May 25 04:20:21 2024, max compression
```

## Comparing `nebulousai-0.1.tar` & `nebulousai-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-19 12:03:34.817685 nebulousai-0.1/
--rw-r--r--   0 admin      (501) staff       (20)     1058 2024-05-19 11:52:17.000000 nebulousai-0.1/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)       74 2024-05-19 12:03:34.817516 nebulousai-0.1/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-19 12:03:34.814215 nebulousai-0.1/nebulousai/
--rw-r--r--   0 admin      (501) staff       (20)       56 2024-05-19 11:32:48.000000 nebulousai-0.1/nebulousai/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1159 2024-05-15 10:22:14.000000 nebulousai-0.1/nebulousai/ability_search.py
--rw-r--r--   0 admin      (501) staff       (20)     5129 2024-05-19 11:40:21.000000 nebulousai-0.1/nebulousai/agent.py
--rw-r--r--   0 admin      (501) staff       (20)     3653 2024-05-19 08:58:49.000000 nebulousai-0.1/nebulousai/all_abilities.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-19 12:03:34.816257 nebulousai-0.1/nebulousai/core/
--rw-r--r--   0 admin      (501) staff       (20)        0 2024-05-19 11:37:10.000000 nebulousai-0.1/nebulousai/core/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      623 2024-05-17 10:43:57.000000 nebulousai-0.1/nebulousai/core/ability.py
--rw-r--r--   0 admin      (501) staff       (20)      355 2024-05-15 10:39:21.000000 nebulousai-0.1/nebulousai/core/brain.py
--rw-r--r--   0 admin      (501) staff       (20)     5256 2024-05-19 09:02:03.000000 nebulousai-0.1/nebulousai/core/planning.py
--rw-r--r--   0 admin      (501) staff       (20)      321 2024-05-15 10:50:46.000000 nebulousai-0.1/nebulousai/core/short_term_memory.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-19 12:03:34.816986 nebulousai-0.1/nebulousai/feedback_loop/
--rw-r--r--   0 admin      (501) staff       (20)        0 2024-05-19 11:37:10.000000 nebulousai-0.1/nebulousai/feedback_loop/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      670 2024-05-13 16:34:42.000000 nebulousai-0.1/nebulousai/feedback_loop/human_feedback.py
--rw-r--r--   0 admin      (501) staff       (20)      152 2024-05-13 16:39:21.000000 nebulousai-0.1/nebulousai/feedback_loop/human_intervention.py
--rw-r--r--   0 admin      (501) staff       (20)      132 2024-05-13 16:38:10.000000 nebulousai-0.1/nebulousai/feedback_loop/learnings.py
--rw-r--r--   0 admin      (501) staff       (20)     1211 2024-04-07 05:46:59.000000 nebulousai-0.1/nebulousai/prompts.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-19 12:03:34.817313 nebulousai-0.1/nebulousai/utils/
--rw-r--r--   0 admin      (501) staff       (20)        0 2024-05-19 11:37:10.000000 nebulousai-0.1/nebulousai/utils/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      193 2024-04-07 05:46:59.000000 nebulousai-0.1/nebulousai/utils/llm.py
--rw-r--r--   0 admin      (501) staff       (20)      464 2024-04-07 05:46:59.000000 nebulousai-0.1/nebulousai/vectordb.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-19 12:03:34.815126 nebulousai-0.1/nebulousai.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)       74 2024-05-19 12:03:34.000000 nebulousai-0.1/nebulousai.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      693 2024-05-19 12:03:34.000000 nebulousai-0.1/nebulousai.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-05-19 12:03:34.000000 nebulousai-0.1/nebulousai.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       58 2024-05-19 12:03:34.000000 nebulousai-0.1/nebulousai.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       11 2024-05-19 12:03:34.000000 nebulousai-0.1/nebulousai.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-05-19 12:03:34.817749 nebulousai-0.1/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)      254 2024-05-19 11:25:20.000000 nebulousai-0.1/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-25 04:20:21.208585 nebulousai-0.1.1/
+-rw-r--r--   0 admin      (501) staff       (20)     1058 2024-05-19 11:52:17.000000 nebulousai-0.1.1/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)     1763 2024-05-25 04:20:21.208424 nebulousai-0.1.1/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-25 04:20:21.205646 nebulousai-0.1.1/nebulousai/
+-rw-r--r--   0 admin      (501) staff       (20)       56 2024-05-19 11:32:48.000000 nebulousai-0.1.1/nebulousai/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     9200 2024-05-25 04:17:14.000000 nebulousai-0.1.1/nebulousai/agent.py
+-rw-r--r--   0 admin      (501) staff       (20)     3592 2024-05-24 07:06:54.000000 nebulousai-0.1.1/nebulousai/all_tools.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-25 04:20:21.207332 nebulousai-0.1.1/nebulousai/core/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-05-19 11:37:10.000000 nebulousai-0.1.1/nebulousai/core/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      355 2024-05-15 10:39:21.000000 nebulousai-0.1.1/nebulousai/core/brain.py
+-rw-r--r--   0 admin      (501) staff       (20)      648 2024-05-22 14:22:34.000000 nebulousai-0.1.1/nebulousai/core/memory.py
+-rw-r--r--   0 admin      (501) staff       (20)     5070 2024-05-24 07:24:46.000000 nebulousai-0.1.1/nebulousai/core/planning.py
+-rw-r--r--   0 admin      (501) staff       (20)      608 2024-05-24 06:42:57.000000 nebulousai-0.1.1/nebulousai/core/tool.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-25 04:20:21.207925 nebulousai-0.1.1/nebulousai/feedback_loop/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-05-19 11:37:10.000000 nebulousai-0.1.1/nebulousai/feedback_loop/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      666 2024-05-24 06:41:41.000000 nebulousai-0.1.1/nebulousai/feedback_loop/human_feedback.py
+-rw-r--r--   0 admin      (501) staff       (20)      152 2024-05-13 16:39:21.000000 nebulousai-0.1.1/nebulousai/feedback_loop/human_intervention.py
+-rw-r--r--   0 admin      (501) staff       (20)      132 2024-05-13 16:38:10.000000 nebulousai-0.1.1/nebulousai/feedback_loop/learnings.py
+-rw-r--r--   0 admin      (501) staff       (20)     1160 2024-05-24 06:42:57.000000 nebulousai-0.1.1/nebulousai/prompts.py
+-rw-r--r--   0 admin      (501) staff       (20)     1074 2024-05-24 06:42:57.000000 nebulousai-0.1.1/nebulousai/tool_search.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-25 04:20:21.208206 nebulousai-0.1.1/nebulousai/utils/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-05-19 11:37:10.000000 nebulousai-0.1.1/nebulousai/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      193 2024-05-22 13:32:23.000000 nebulousai-0.1.1/nebulousai/utils/llm.py
+-rw-r--r--   0 admin      (501) staff       (20)      440 2024-05-24 06:41:59.000000 nebulousai-0.1.1/nebulousai/vectordb.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-25 04:20:21.206507 nebulousai-0.1.1/nebulousai.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1763 2024-05-25 04:20:21.000000 nebulousai-0.1.1/nebulousai.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      672 2024-05-25 04:20:21.000000 nebulousai-0.1.1/nebulousai.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-05-25 04:20:21.000000 nebulousai-0.1.1/nebulousai.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       58 2024-05-25 04:20:21.000000 nebulousai-0.1.1/nebulousai.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       11 2024-05-25 04:20:21.000000 nebulousai-0.1.1/nebulousai.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-05-25 04:20:21.208649 nebulousai-0.1.1/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)      401 2024-05-25 04:06:16.000000 nebulousai-0.1.1/setup.py
```

### Comparing `nebulousai-0.1/LICENSE` & `nebulousai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebulousai-0.1/nebulousai/ability_search.py` & `nebulousai-0.1.1/nebulousai/tool_search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from .prompts import AbilitySearchPrompt
+from .prompts import ToolSearchPrompt
 from .utils.llm import llm_call
 from .vectordb import vector_search, get_embedding
 
 import json
 
-def search_ability(abilities, task, method):
+def search_tool(tools, task, method):
     # Placeholder for different search mechanisms
     if method == "llm_call":
-        ability_search_prompt = AbilitySearchPrompt(abilities).generate_prompt()
-        messages = [{"role" : "system", "content" : ability_search_prompt},
+        tool_search_prompt = ToolSearchPrompt(tools).generate_prompt()
+        messages = [{"role" : "system", "content" : tool_search_prompt},
                     {"role" : "user", "content" : task}]
-        best_matching_ability_object = llm_call(messages, "gpt-3.5-turbo")
-        best_matching_ability_object = json.loads(best_matching_ability_object)
-        print(best_matching_ability_object)
+        best_matching_tool_object = llm_call(messages, "gpt-3.5-turbo")
+        best_matching_tool_object = json.loads(best_matching_tool_object)
+        print(best_matching_tool_object)
 
-        ability_name = best_matching_ability_object.pop("ability_name")
-        best_matching_ability = [ability for ability in abilities if ability.ability_name == ability_name][0]
-        best_matching_ability.args = best_matching_ability_object
+        tool_name = best_matching_tool_object.pop("tool_name")
+        best_matching_tool = [tool for tool in tools if tool.tool_name == tool_name][0]
+        best_matching_tool.args = best_matching_tool_object
 
-        return best_matching_ability
+        return best_matching_tool
 
     elif method == "vector_search":
         task_embedding = get_embedding(task)
-        best_matching_ability = vector_search(abilities, task_embedding)
-        return best_matching_ability
+        best_matching_tool = vector_search(tools, task_embedding)
+        return best_matching_tool
```

### Comparing `nebulousai-0.1/nebulousai/all_abilities.py` & `nebulousai-0.1.1/nebulousai/all_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 import wikipedia
 import requests
 from bs4 import BeautifulSoup
 from duckduckgo_search import DDGS
 
 from .utils.llm import llm_call
-from .core.ability import Ability
+from .core.tool import Tool
+
+# Symbolic Modules
 
 def search_wikipedia(search_term:str):
     search_results = wikipedia.search(search_term)
     selected_search_result = search_results[0]
     page_summary = wikipedia.summary(selected_search_result)
     #page = wikipedia.page(search_term)
     return page_summary #page.content#, , page.links
 
-search_wikipedia_ability_description = """Searches Wikipedia using the API to return the page summary, page content and list of links.
+search_wikipedia_tool_description = """Searches Wikipedia using the API to return the page summary, page content and list of links.
 You must ensure that a page for your entered search term exists on Wikipedia.
 Use the returned page content, pass it through the reasoning step with a question to get your answer."""
 
-searchWikipediaAbility = Ability(ability_name="Wikipedia Search",
-                                 description=search_wikipedia_ability_description,
+searchWikipediaTool = Tool(tool_name="Wikipedia Search",
+                                 description=search_wikipedia_tool_description,
                                  action=search_wikipedia)
 
 
 
 
 def reason(input_text:str):
     return llm_call([{"role" : "user", "content" : input_text}])
 
-reason_ability_description = """Makes an LLM call to figure out an answer.
+reason_tool_description = """Makes an LLM call to figure out an answer.
 In the input text string, make sure that you include all the relevant context and clearly mention your question and the expected output from the LLM.
 """
 
-reasonAbility = Ability(ability_name = "Reason",
-                        description = reason_ability_description,
+reasonTool = Tool(tool_name = "Reason",
+                        description = reason_tool_description,
                         action=reason)
 
 
 
 def web_search_ddg(search_term:str):
     results = DDGS().text(search_term, max_results=5)
     return str(results)
 
-web_search_ddg_ability_description = """Given a search query, searches the DuckDuckGo search engine.
+web_search_ddg_tool_description = """Given a search query, searches the DuckDuckGo search engine.
 Returns 5 search results with the title, URL and a few sentences of the body, of each search result.
-After getting the search results, the agent should usually use the getWebpageContentAbility to visit the most relevant URL, read its content, and answer the user's question.
+The search results are only useful if, after searching, the agent uses the getWebpageContentTool to visit the most relevant URL, reads its content, and finds the answer to the user's question.
 """
 
-webSearchAbility = Ability(ability_name="Web Search",
-                           description=web_search_ddg_ability_description,
+webSearchTool = Tool(tool_name="Web Search",
+                           description=web_search_ddg_tool_description,
                            action=web_search_ddg)
 
 
 
 def get_webpage_content(url:str):
     try:
         response = requests.get(url)
@@ -59,28 +61,28 @@
         soup = BeautifulSoup(response.content, 'html.parser')
         title = soup.title.string if soup.title else 'No title found'
         text_content = ' '.join(soup.stripped_strings)
         return f"{title}\n{text_content}"
     except requests.exceptions.RequestException as e:
         return "There was an error reading this webpage."
 
-get_webpage_content_ability_description = """Given the URL to a webpage, returns the page content if it is accessible.
-Before using this ability, you would usually have searched the web to have your search results' URLs ready.
-The Web Search Ability's response only contains page titles and a few sentences. So, if these sentences do not answer the user's question, you must visit one of the webpage URLs to get the full text.
-After using this ability, you can use the Reasoning ability to filter / summarise the text to generate the final answer for the user.
+get_webpage_content_tool_description = """Given the URL to a webpage, returns the page content if it is accessible.
+Before using this tool, you would usually have searched the web to have your search results' URLs ready.
+The Web Search Tool's response only contains page titles and a few sentences. So, if these sentences do not answer the user's question, you must visit one of the webpage URLs to get the full text.
+After using this tool, you can use the Reasoning tool to filter / summarise the text to generate the final answer for the user.
 If a certain webpage's content is not accessible, the agent must try another search result URL.
 """
 
-getWebpageContentAbility = Ability(ability_name = "Get Webpage Content",
-                        description = get_webpage_content_ability_description,
+getWebpageContentTool = Tool(tool_name = "Get Webpage Content",
+                        description = get_webpage_content_tool_description,
                         action=get_webpage_content)
 
 
 
 
 #Human Feedback
 
 def send_email(name:str, email_address:str, email_subject:str, email_body:str):
-    return "sent email"
+    pass #TODO
 
 def poll_for_email_reply():
-    return "received email"
+    pass #TODO
```

### Comparing `nebulousai-0.1/nebulousai/core/ability.py` & `nebulousai-0.1.1/nebulousai/core/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from ..vectordb import get_embedding
-class Ability:
-    def __init__(self, ability_name, description, action, args=[]):
-        self.ability_name = ability_name
+class Tool:
+    def __init__(self, tool_name, description, action, args=[]):
+        self.tool_name = tool_name
         self.description = description
         #self.description_embedding = get_embedding(description)
         self.action = action
         self.args = args
 
-class Instruction(Ability):
+class Instruction(Tool):
     def __init__(self, instruction_name, description, func, args, response_variable):
         self.instruction_name = instruction_name
         self.description = description
         self.func = func
         self.args = args
         self.response_variable = response_variable
```

### Comparing `nebulousai-0.1/nebulousai/core/planning.py` & `nebulousai-0.1.1/nebulousai/core/planning.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 class Planner:
     def __init__(self, agent_goal, refine_plan=False):
         self.agent_goal = agent_goal
         self.refine_plan = refine_plan
         self.agent_plan_steps = []
 
     #Decomposition into subgoals
-    def decompose_tasks_into_subtasks(self, abilities, brain):
+    def decompose_tasks_into_subtasks(self, tools, brain):
                 
-        abilities = '\n\n'.join([f"- {ability.ability_name}\n{ability.description}" for ability in abilities])
+        tools = '\n\n'.join([f"- {tool.tool_name}\n{tool.description}" for tool in tools])
         chain_of_thought_planning_prompt = f"""
         You are given a task the user wants to accomplish. These are the guidelines the user has set for you:
         {brain.brain_system_prompt}
 
-        You have the following abilities you can use to complete this task:
-        {abilities}
+        You have the following tools you can use to complete this task:
+        {tools}
 
         Plan out a series of steps that allow you to complete this task. You can plan any number of tasks.
-        In each step, name the ability to be used, and its input and expected output.
+        In each step, name the tool to be used, and its input and expected output.
         Return your response in the below format. Do not add any comments in your response or it will not be parsed correctly!
 
         Step 1:
         Function, reason for using this function, input to function, expected output.
 
         Step 2:
         Function, reason for using this function, input to function, expected output.
@@ -41,62 +41,60 @@
                     {"role" : "user", "content" : self.agent_goal}]
         
         llm_response_plan = llm_call(messages)
         steps = re.findall(r'Step \d+:(.*?)(?=Step \d+|$)', llm_response_plan, re.DOTALL)
         self.agent_plan_steps = [step.strip() for step in steps]
 
 
-    def convert_plan_step_to_instruction(self, plan_step, abilities, retries=5):
-        abilities_definition_str = ""
-        for ability in abilities:
-            params = inspect.signature(ability.action).parameters.values()
+    def convert_plan_step_to_instruction(self, plan_step, tools, retries=5):
+        tools_definition_str = ""
+        for tool in tools:
+            params = inspect.signature(tool.action).parameters.values()
             params_str = "\n".join([f'Name: {param.name}, Default: {param.default}, Kind: {param.kind}' for param in params])
-            abilities_definition_str += f"""\n\nTool: {ability.ability_name}\nDescription: {ability.description}\nArguments: {params_str}"""
+            tools_definition_str += f"""\n\nTool: {tool.tool_name}\nDescription: {tool.description}\nArguments: {params_str}"""
         
-        #print(abilities_definition_str)
         convert_plan_to_instructions_system_prompt = f"""
         You are part of an AI agent flow. The user will give you an action they want to perform.
         You also have a set of tools to perform it.
         FIgure out the appropriate tool and the input to be given to it.
 
         <available tools>
-        - {abilities_definition_str}
+        - {tools_definition_str}
         </available tools>
 
         Return your response in the below JSON format. Do not add any comments in your response or it will not be parsed correctly!
-        """ + """{"ability_name" : "abilityName1",
+        """ + """{"tool_name" : "toolName1",
          "arguments" : {"argument_1_name" : "argument_1_value", "argument_2_name" : "argument_2_value"}
         }"""
         
         convert_plan_to_instructions_system_prompt = convert_plan_to_instructions_system_prompt.replace("    ", "")
         try:
             messages = [{"role" : "system", "content" : convert_plan_to_instructions_system_prompt},
                         {"role" : "user", "content" : plan_step}]
             
             instructions_llm_response = llm_call(messages)
             instructions_llm_response_parsed = json.loads(instructions_llm_response)
         except JSONDecodeError:
-            print(instructions_llm_response)
-            if retries > 0: return self.convert_plan_step_to_instruction(plan_step, abilities, retries-1)
+            if retries > 0: return self.convert_plan_step_to_instruction(plan_step, tools, retries-1)
         return instructions_llm_response_parsed
     
 
     #Reflection and refinement
-    def reflect_upon_and_refine_plan_llm_call(plan, abilities):
+    def reflect_upon_and_refine_plan_llm_call(plan, tools):
         reflect_upon_and_refine_plan_system_prompt = ""
         messages = [{"role" : "system", "content" : reflect_upon_and_refine_plan_system_prompt},
                     {"role" : "user", "content" : plan}]
         
         instructions_llm_response = llm_call(messages)
         instructions_llm_response = instructions_llm_response.split("\n")
         return instructions_llm_response
     
 
-    def plan_task(self, abilities, brain):
-        self.decompose_tasks_into_subtasks(abilities=abilities, brain=brain)
+    def plan_task(self, tools, brain):
+        self.decompose_tasks_into_subtasks(tools=tools, brain=brain)
         if self.refine_plan: self.reflect_upon_and_refine_plan_llm_call()
 
     
     def from_preplanned_steps(self, plan_steps):
         self.agent_plan_steps = plan_steps
 
 
@@ -104,12 +102,12 @@
 
 class TreeOfThoughtPlanner:
     def __init__(self, agent_goal, refine_plan=False):
         self.agent_goal = agent_goal
         self.refine_plan = refine_plan
         self.agent_plan_steps = []
 
-    def decompose_tasks_into_subtasks(self, abilities):
+    def decompose_tasks_into_subtasks(self, tools):
         tree_of_thought_prompt = """"""
         # exploring multiple reasoning possibilities at each step. It first decomposes the problem into multiple thought steps and generates multiple thoughts per step, creating a tree structure. The search process can be BFS (breadth-first search) or DFS (depth-first search) with each state evaluated by a classifier (via a prompt) or majority vote.
         # https://arxiv.org/abs/2305.10601
         pass
```

### Comparing `nebulousai-0.1/nebulousai/feedback_loop/human_feedback.py` & `nebulousai-0.1.1/nebulousai/feedback_loop/human_feedback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from all_abilities import send_email
+from all_tools import send_email
 
 class PointOfContact:
     def __init__(self, point_of_contact_name, communication_mode, communication_address) -> None:
         self.point_of_contact_name = point_of_contact_name
         self.communication_address = communication_address
         self.communication_mode = communication_mode
```

### Comparing `nebulousai-0.1/nebulousai/prompts.py` & `nebulousai-0.1.1/nebulousai/prompts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-class AbilitySearchPrompt:
-    def __init__(self, abilities):
-        self.abilities = abilities
+class ToolSearchPrompt:
+    def __init__(self, tools):
+        self.tools = tools
 
     def generate_prompt(self):
         prompt = """
         You are part of an autonomous agent.
-        You are provided with a list of abilities the agent has. The user will provide a task they want to accomplish.
-        You will return the name of the most suitable ability to be used for this task, as well as the values of the arguments to be plugged in.
+        You are provided with a list of tools the agent has. The user will provide a task they want to accomplish.
+        You will return the name of the most suitable tool to be used for this task, as well as the values of the arguments to be plugged in.
         
-        # Example ability:
+        # Example tool:
         create_sheet: Creates a new worksheet.
         Arguments: sheet_name, company_name
 
         # Example user task:
         - Make a sheet named Sarthak for OpenAI.
 
         # Example response:
-        {"ability_name" : "create_sheet", "sheet_name" : "Sarthak", "company_name" : "OpenAI"}
+        {"tool_name" : "create_sheet", "sheet_name" : "Sarthak", "company_name" : "OpenAI"}
 
         Return your response strictly in the above JSON format. Only return this JSON and nothing else.
         Do not add any comments or explanations, or your response will not be parsed correctly.
-        Below are the abilities:
+        Below are the tools:
         - """
 
-        prompt += "\n".join([f"- {ability.ability_name}: {ability.description}\nArguments: {', '.join(ability.args)}\n" for ability in self.abilities])
+        prompt += "\n".join([f"- {tool.tool_name}: {tool.description}\nArguments: {', '.join(tool.args)}\n" for tool in self.tools])
         return prompt
```

### Comparing `nebulousai-0.1/nebulousai.egg-info/SOURCES.txt` & `nebulousai-0.1.1/nebulousai.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 LICENSE
 setup.py
 nebulousai/__init__.py
-nebulousai/ability_search.py
 nebulousai/agent.py
-nebulousai/all_abilities.py
+nebulousai/all_tools.py
 nebulousai/prompts.py
+nebulousai/tool_search.py
 nebulousai/vectordb.py
 nebulousai.egg-info/PKG-INFO
 nebulousai.egg-info/SOURCES.txt
 nebulousai.egg-info/dependency_links.txt
 nebulousai.egg-info/requires.txt
 nebulousai.egg-info/top_level.txt
 nebulousai/core/__init__.py
-nebulousai/core/ability.py
 nebulousai/core/brain.py
+nebulousai/core/memory.py
 nebulousai/core/planning.py
-nebulousai/core/short_term_memory.py
+nebulousai/core/tool.py
 nebulousai/feedback_loop/__init__.py
 nebulousai/feedback_loop/human_feedback.py
 nebulousai/feedback_loop/human_intervention.py
 nebulousai/feedback_loop/learnings.py
 nebulousai/utils/__init__.py
 nebulousai/utils/llm.py
```

