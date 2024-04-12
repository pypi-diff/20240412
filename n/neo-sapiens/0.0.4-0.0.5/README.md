# Comparing `tmp/neo_sapiens-0.0.4.tar.gz` & `tmp/neo_sapiens-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo_sapiens-0.0.4.tar", max compression
+gzip compressed data, was "neo_sapiens-0.0.5.tar", max compression
```

## Comparing `neo_sapiens-0.0.4.tar` & `neo_sapiens-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-04-07 22:57:58.790247 neo_sapiens-0.0.4/LICENSE
--rw-r--r--   0        0        0      315 2024-04-10 14:58:18.826324 neo_sapiens-0.0.4/README.md
--rw-r--r--   0        0        0      455 2024-04-10 14:50:26.476068 neo_sapiens-0.0.4/neo_sapiens/__init__.py
--rw-r--r--   0        0        0     6423 2024-04-10 14:52:15.126745 neo_sapiens-0.0.4/neo_sapiens/few_shot_prompts.py
--rw-r--r--   0        0        0     6732 2024-04-10 14:49:59.540629 neo_sapiens-0.0.4/neo_sapiens/hass_schema.py
--rw-r--r--   0        0        0     1342 2024-04-10 14:58:27.026683 neo_sapiens-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 neo_sapiens-0.0.4/setup.py
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 neo_sapiens-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-07 22:57:58.790247 neo_sapiens-0.0.5/LICENSE
+-rw-r--r--   0        0        0      927 2024-04-11 21:29:42.173625 neo_sapiens-0.0.5/README.md
+-rw-r--r--   0        0        0      456 2024-04-11 21:29:42.231609 neo_sapiens-0.0.5/neo_sapiens/__init__.py
+-rw-r--r--   0        0        0     5530 2024-04-11 21:29:42.232687 neo_sapiens-0.0.5/neo_sapiens/chroma_db_s.py
+-rw-r--r--   0        0        0     6961 2024-04-11 22:50:25.412884 neo_sapiens-0.0.5/neo_sapiens/few_shot_prompts.py
+-rw-r--r--   0        0        0     8588 2024-04-12 01:52:27.925780 neo_sapiens-0.0.5/neo_sapiens/hass_schema.py
+-rw-r--r--   0        0        0     1647 2024-04-12 01:51:46.306911 neo_sapiens-0.0.5/neo_sapiens/tools_preset.py
+-rw-r--r--   0        0        0     1342 2024-04-12 01:53:25.567067 neo_sapiens-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 neo_sapiens-0.0.5/setup.py
+-rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 neo_sapiens-0.0.5/PKG-INFO
```

### Comparing `neo_sapiens-0.0.4/LICENSE` & `neo_sapiens-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neo_sapiens-0.0.4/neo_sapiens/few_shot_prompts.py` & `neo_sapiens-0.0.5/neo_sapiens/few_shot_prompts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import List
 
 # Example usage
 data = """
 {
     "plan": ["Step 1", "Step 2", "Step 3"],
-    "number_of_agents": 5,
     "agents": [
         {
             "name": "Agent 1",
             "system_prompt": "Prompt 1"
         },
         {
             "name": "Agent 2",
@@ -18,15 +17,14 @@
 }
 """
 
 # AI Research Team 1
 data1 = """
 {
     "plan": ["Data Collection", "Data Cleaning", "Model Training", "Model Evaluation"],
-    "number_of_agents": 3,
     "agents": [
         {
             "name": "Data Agent",
             "system_prompt": "Collect and clean data"
         },
         {
             "name": "Training Agent",
@@ -40,15 +38,14 @@
 }
 """
 
 # AI Research Team 2
 data2 = """
 {
     "plan": ["Literature Review", "Hypothesis Formulation", "Experiment Design", "Data Analysis", "Paper Writing"],
-    "number_of_agents": 5,
     "agents": [
         {
             "name": "Review Agent",
             "system_prompt": "Review the literature"
         },
         {
             "name": "Hypothesis Agent",
@@ -70,15 +67,14 @@
 }
 """
 
 # AI Research Team 3
 data3 = """
 {
     "plan": ["Problem Identification", "Solution Design", "Implementation", "Testing", "Deployment"],
-    "number_of_agents": 4,
     "agents": [
         {
             "name": "Identification Agent",
             "system_prompt": "Identify the problem"
         },
         {
             "name": "Design Agent",
@@ -96,15 +92,14 @@
 }
 """
 
 
 data5 = """
 {
     "plan": ["Room Management", "Guest Services", "Reservations Handling", "Facility Maintenance", "Staff Coordination"],
-    "number_of_agents": 5,
     "agents": [
         {
             "name": "Room Management Agent",
             "system_prompt": "Automate room assignments, minibar restocking, and housekeeping schedules"
         },
         {
             "name": "Guest Services Agent",
@@ -138,17 +133,14 @@
 
     Returns:
         str: The merged plans as a single string.
     """
     return "\n".join(plan)
 
 
-
-
-
 self_driving_car_prompt = """
 
 {
     "plan": [
         (
             "Step 1: Create agents specialized in different areas"
             " like computer vision, sensor fusion, controls,"
@@ -170,15 +162,14 @@
         ),
         (
             "Step 5: Integrate components into a complete"
             " self-driving system and validate performance through"
             " simulation and real-world testing"
         ),
     ],
-    "number_of_agents": 5,
     "agents": [
         {
             "name": "Computer Vision Agent",
             "system_prompt": (
                 "Create an AI agent specialized in computer vision"
                 " for self-driving cars, focused on object detection,"
                 " segmentation and tracking using deep learning"
@@ -200,26 +191,42 @@
     ],
 }
 
 
 """
 
 
-
-
 def orchestrator_prompt_agent(objective: str):
     prompt = (
         "Create an instruction prompt for an swarm orchestrator to"
         " create a series of personalized, agents for the following"
         f" objective: {objective} to decompose a very complicated"
         " problem or tasks, the orchestrator is the team leader."
         " Teach the orchestrator how to decompose the tasks to very"
         " certain agents with names, and system prompts, we need the"
         " plan, with a step by stpe instructions, number of agents,"
         " and a list of agents with a name, system prompt for each,"
         " and then the rules of the swarm,  compact the prompt, and"
-        " say only return JSON data in markdown and nothing else."
-        f"Follow the schema here: {data} *############ Here are some examples:"
-        f"{data5} and another example{data3} "
-        
+        " say only return JSON data in markdown and nothing"
+        f" else.Follow the schema here: {data} *############ Here are"
+        f" some examples:{data5} and another example{data3} "
     )
     return str(prompt)
+
+
+boss_sys_prompt = (
+    "You're the Swarm Orchestrator, like a project manager of a"
+    " bustling hive. When a task arises, you tap into your network of"
+    " worker agents who are ready to jump into action. Whether it's"
+    " organizing data, handling logistics, or crunching numbers, you"
+    " delegate tasks strategically to maximize efficiency. Picture"
+    " yourself as the conductor of a well-oiled machine,"
+    " orchestrating the workflow seamlessly to achieve optimal"
+    " results with your team of dedicated worker agents."
+)
+
+
+def select_workers(agents: str, task: str):
+    return (
+        f"These are the agents available for the task: {task} Agents"
+        f" available: {agents}"
+    )
```

### Comparing `neo_sapiens-0.0.4/neo_sapiens/hass_schema.py` & `neo_sapiens-0.0.5/neo_sapiens/hass_schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,49 @@
 import json
 import os
 import re
 from typing import List
 
 from dotenv import load_dotenv
 from pydantic import BaseModel, Field
-from swarms import Agent, Anthropic, SwarmNetwork
+from swarms import Agent, Anthropic, SwarmNetwork, tool
 
 from neo_sapiens.few_shot_prompts import (
     data,
     data1,
     data2,
     data3,
     orchestrator_prompt_agent,
+    select_workers,
+    boss_sys_prompt,
+)
+from loguru import logger
+from neo_sapiens.tools_preset import (
+    terminal,
+    browser,
+    file_editor,
+    create_file,
 )
 
 # Load environment variables
 load_dotenv()
 
 # Swarmnetowr
 network = SwarmNetwork(api_enabled=True, logging_enabled=True)
 
 
+# Initialize memory
+# memory = ChromaDB(
+#     metric="cosine",
+#     output_dir="swarms",
+#     limit_tokens=1000,
+#     n_results=2,
+#     verbose=False,
+# )
+
 # def tool_router(tool: str, *args, **kwargs):
 #     if "terminal" in tool:
 #         return terminal(*args, **kwargs)
 #     elif "browser" in tool:
 #         return browser(*args, **kwargs)
 
 
@@ -35,17 +53,16 @@
 
     Args:
         name (str): The name of the agent.
 
     Returns:
         str: The ID of the agent.
     """
-    agents = network.list_agents()
-    for agent in agents:
-        if agent.name == name:
+    for agent in network.agent_pool:
+        if agent.agent_name == name:
             return agent.id
 
 
 class ToolSchema(BaseModel):
     tool: str = Field(
         ...,
         title="Tool name",
@@ -79,19 +96,14 @@
 
 class HassSchema(BaseModel):
     plan: List[str] = Field(
         ...,
         title="Plan to solve the input problem",
         description="List of steps to solve the problem",
     )
-    number_of_agents: int = Field(
-        ...,
-        title="Number of agents to use for the problem",
-        description="Number of agents to use for the problem",
-    )
     agents: List[AgentSchema] = Field(
         ...,
         title="List of agents to use for the problem",
         description="List of agents to use for the problem",
     )
     # Rules for the agents
     # rules: str = Field(
@@ -101,35 +113,32 @@
     # )
 
 
 # import json
 def parse_json_from_input(input_str):
     # Validate input is not None or empty
     if not input_str:
-        print("Error: Input string is None or empty.")
+        logger.info("Error: Input string is None or empty.")
         return None, None, None
 
     # Attempt to extract JSON from markdown using regular expression
     json_pattern = re.compile(r"```json\n(.*?)\n```", re.DOTALL)
     match = json_pattern.search(input_str)
     json_str = match.group(1).strip() if match else input_str.strip()
-    # print(json_str)
 
     # Attempt to parse the JSON string
     try:
         data = json.loads(json_str)
-        # print(str(data))
     except json.JSONDecodeError as e:
-        print(f"Error: JSON decoding failed with message '{e}'")
+        logger.info(f"Error: JSON decoding failed with message '{e}'")
         return None, None, None
 
     hass_schema = HassSchema(**data)
     return (
         hass_schema.plan,
-        hass_schema.number_of_agents,
         hass_schema.agents,
         # hass_schema.rules,
     )
 
 
 # You can test the function with a markdown string similar to the one provided.
 
@@ -164,113 +173,183 @@
         str: The merged prompts as a single string.
     """
     return "\n".join(prompts)
 
 
 def create_agents(
     agents: List[AgentSchema],
-):
+) -> List[Agent]:
     """
     Create and initialize agents based on the provided AgentSchema objects.
 
     Args:
         agents (List[AgentSchema]): A list of AgentSchema objects containing agent information.
 
     Returns:
-        Agent: The initialized Agent object.
+        List[Agent]: The initialized Agent objects.
 
     """
+    agent_list = []
     for agent in agents:
-        print(agent)
         name = agent.name
         system_prompt = agent.system_prompt
-        print(agent.name)
-        print(agent.system_prompt)
-        print("\n")
+
+        logger.info(
+            f"Creating agent: {name} with system prompt:"
+            f" {system_prompt}"
+        )
 
         out = Agent(
             agent_name=name,
             system_prompt=system_prompt,
             llm=Anthropic(
                 anthropic_api_key=os.getenv("ANTHROPIC_API_KEY")
             ),
             max_loops=1,
             autosave=True,
             dashboard=False,
             verbose=True,
             stopping_token="<DONE>",
-            interactive=True,
+            tools=[browser, terminal, create_file, file_editor],
         )
 
         network.add_agent(out)
+        agent_list.append(out)
+
+    return agent_list
 
-    return out
 
+def print_agent_names(agents: list):
+    for agent in agents:
+        logger.info(f"Agent Name: {agent.agent_name}")
 
-# out = create_agents(agents)
-# # print(out)
 
-# # # Use network
-# # list_agents = network.list_agents()
-# # print(list_agents)
-
-# # Run the workflow on a task
-# run = network.run_single_agent(
-#     agent2.id, "What's your name?"
-# )
-# print(out)
+@tool
+def send_task_to_network_agent(name: str, task: str):
+    """
+    Send a task to a network agent.
+
+    Args:
+        name (str): The name of the agent.
+        task (str): The task to be sent to the agent.
+
+    Returns:
+        str: The response from the agent.
+    """
+    logger.info(f"Adding agent {name} as a tool")
+    agent_id = find_agent_id_by_name(name)
+    out = network.run_single_agent(agent_id, task)
+    return out
 
 
-def run_swarm(task: str = None):
+def master_creates_agents(task: str, *args, **kwargs):
     """
-    Run a task using the Swarm Orchestrator agent.
+    Master function to create agents based on a task.
 
     Args:
         task (str): The task to be executed.
 
     Returns:
         None
     """
     system_prompt_daddy = orchestrator_prompt_agent(task)
-    # print(system_prompt_daddy)
+
+    # Create the agents
     agent = Agent(
         agent_name="Swarm Orchestrator",
         system_prompt=system_prompt_daddy,
         llm=Anthropic(
             anthropic_api_key=os.getenv("ANTHROPIC_API_KEY"),
             max_tokens=4000,
         ),
         max_loops=1,
         autosave=True,
         dashboard=False,
         verbose=True,
         stopping_token="<DONE>",
-        # interactive=True,
+        *args,
+        **kwargs,
+    )
+
+    # Call the agents [ Main Agents ]
+    # Create the agents
+    boss = Agent(
+        agent_name="Swarm Orchestrator",
+        system_prompt=boss_sys_prompt,
+        llm=Anthropic(
+            anthropic_api_key=os.getenv("ANTHROPIC_API_KEY"),
+            max_tokens=4000,
+        ),
+        max_loops="auto",
+        autosave=True,
+        dashboard=False,
+        verbose=True,
+        stopping_token="<DONE>",
+        interactive=True,
+        *args,
+        **kwargs,
     )
-    out = agent.run(task)
-    # print(out)
-    out = str(out)
-    print(f"Output: {out}")
+
+    # Task 1: Run the agent and parse the output
+    logger.info("Creating the workers ...")
+    out = agent.run(str(task))
+    # logger.info(f"Output: {out}")
     out = parse_json_from_input(out)
-    print(str(out))
-    plan, number_of_agents, agents = out
-    print(agents)
+    json_agentic_output = out
+    # logger.info(str(out))
+    plan, agents = out
+
+    # Task 2: Print agent names and create agents
+    # logger.info(agents)
+    # logger.info("Creating agents...")
     agents = create_agents(agents)
-    print(agents)
-    # return agents
-    # print(out)
-    # json_template = extract_code_from_markdown(str(out))
-    # print(json_template)
-    # parsed_schema = parse_json_from_markdown(json_template)
-    # plan, number_of_agents, agents = parsed_schema
-    # print(f"Plan: {agents}")
-    # # agents = create_agents(agents)
-    # print(agents)
-    # return agents
-    return out
 
+    # Send JSON of agents to boss
+    boss.add_message_to_memory(
+        select_workers(json_agentic_output, task)
+    )
+
+    # Task 3: Now add the agents as tools
+    boss.add_tool(send_task_to_network_agent)
 
-# out = run_task(
-#     "Create a team of AI engineers to create an AI for a"
-#     " self-driving car"
-# )
-# # print(out)
+    # Run the boss:
+    out = boss.run(task)
+
+    return out  # , agents, plan
+
+
+def message_metadata_log(task: str, message: str, agent, plan: str):
+    """
+    Create a document with metadata for a log message.
+
+    Args:
+        task (str): The task associated with the log message.
+        message (str): The log message.
+        agent: The agent object.
+        plan (str): The plan associated with the log message.
+
+    Returns:
+        dict: A dictionary containing the log message metadata.
+    """
+    doc = {
+        "message": message,
+        "task": task,
+        "agent_name": agent.agent_name,
+        "plan": plan,
+    }
+
+    return doc
+
+
+def run_swarm(task: str = None, *args, **kwargs):
+    """
+    Run a task using the Swarm Orchestrator agent.
+
+    Args:
+        task (str): The task to be executed.
+
+    Returns:
+        None
+    """
+    out = master_creates_agents(task, *args, **kwargs)
+    # return passed
+    return out
```

### Comparing `neo_sapiens-0.0.4/pyproject.toml` & `neo_sapiens-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "neo-sapiens"
-version = "0.0.4"
+version = "0.0.5"
 description = "Neo Sapiens - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/NeoSapiens"
 documentation = "https://github.com/kyegomez/NeoSapiens"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/NeoSapiens"
```

