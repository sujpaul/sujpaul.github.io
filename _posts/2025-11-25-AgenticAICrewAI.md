---
title: "Creating a Report Summary with CrewAI- framework for AgenticAI"
date: 2025-11-25
categories: [AgenticAI, CrewAI, Organizational Behaviour, Persistence, Cognition, Action]
tags: [AgentAI, LLM,AgencticAI, CrewAI]
read_time: true          # Shows estimated reading time (e.g., "7 min read")
toc: true                # Enables Table of Contents
toc_sticky: true         # Keeps TOC visible as you scroll (nice for long posts)
comments: false
---

## Introduction

In this blog I will be exploring the use of Agentic AI. I will explore how it can be used, for example, to summarize one of my previous blogs.  There are a few frameworks that can be used : CrewAI, LangGraph, Autogen and SemanticKernel. However, in this article I will be using the CrewAI framework.  This is very much a technical article where the value resides in how effectively and efficiently the Agentic AI can craft a summary of an earlier blog that I had written.  Definitely, from an operation perspective and as a use case, I can see when an executive asks for a summary of any article or a presentation how quickly you can generate and help facilitate the process.  This can also be used as a quick win to show the powers to be what can be achieved and then scale up the operation. 

## What Is Agentic AI

With the progression from the initial usage of static prompt response from LLM to specific task enabled response in the usage of AI Agents, the evolutionary progress to dynamic Agentic AI where multi-agent systems (MAS) can work together in collaborative, competitive or hybrid format has made it an attractive technology to achieve overall objectives.  There are 5 types of agents: Simple Reflex agents, model-based reflex agent, Goal-based agents, Utility-based agents and Learning agents[1]. LLM (Large Language Model)-based agents, as with RL-agents, fall under the category of Learning agents.  A fundamental characteristic of a learning agent is its ability to learn and from its experience improve its behaviour.  This enables the agents to improves its decision-making abilities and drives its autonomous behaviour.
Cheng et al [1] states that “ any entity capable of perceiving its environment and taking action can be considered an agent. Agents have the autonomy to carry out tasks in diverse environments, relying on their past experiences and knowledge to make decisions that align with predefined objectives.”
Agents generally exhibit the following characteristics as mentioned in the above statement:
•	Perception: This is where the model tries to interpret or perceive the environment by extracting the raw input data and converting to meaningful data structures for making decisions
•	Decision-making:  This is where it tries to understand the goal before the tasks start to plan and break it down. Tasks are prioritized and reasoning happens without external intervention. It also tries to manage uncertainty and adaptability. 
•	Action: This is where the tasks are executed and modifies the environment based on the decisions.  It uses various tools to deliver a formatted output. 
•	Autonomy:  The agent makes use of both the decision-making and action characteristics.  It is here that it decides to augment and self-correct its behaviour by self-learning and other tools like (react, reflexion, plan-execute)

Agentic AI, therefore, represents an evolution from traditional AI agents by integrating the strengths of LLMs with the adaptive and reflective capacities of agents. This synergy allows Agentic AI to not only perform tasks autonomously but also to learn from interactions, adjust strategies in real-time, and collaborate effectively with other agents or humans. By leveraging both structured reasoning and flexible problem-solving, Agentic AI stands out as a more dynamic and capable approach within the field of artificial intelligence. The difference between Agentic AI and AI Agents are shown in the following Figure 1.[5]

Figure 1 Difference between AI agents and Agentic AI

![AgenticAI](/assets/images/intro_strategy/media/AgenticAIAgentsDifferences.png)

Figure 1 Difference between AI agents and Agentic AI

LLMs by its very nature has the ability to understand natural language processing.  This along with the vast knowledge across different domains that it accrued as a result of training makes the joining of agents and LLMs a powerful tool.  Agentic AI can then use LLM or action to harness the knowledge and reasoning while being able to reflect and rethink once it gets the response.  Scouring the environment helps the Agentic AI with learning to learn like the learning process that we do in our everyday life.  It is this reflective ability and hence adaptability of Agentic AI that adds to the already 4 characteristics listed above.  The continuous improvement (CI) and learning through the use of ML, DL and other multi-modal LLM available. This added strength of Agentic AI where you let the agents to rationalize, make intelligent decisions and then able to rectify its own decisions by introspection (2) , able to store in memory(3) to access previous information and updates its knowledge regularly have been a major contributor in the fields of self-driving cars and laboratories.  

The 5 components of LLM-based agents are: LLM, Objective, Action, Memory and Rethink.  The LLM is the cerebral component of the agent.  This is actually powered by the initial prompt and makes use of its already existing knowledge to access the domain. The objective is the goal that the agent is set to achieve.  Memory comprises of short-term, long-term and episodic memory. The constituent parts of each of the agents then actions the tools to interact with the external environment.  Tools like API, web sources, database queries are used to access the environments like IOT, coding.  The feedback is provided to the agent to reflect on its actions and then using any of the feedback loop actions then improves on its learning process.  As such access to the appropriate tools is critical in helping the agent to automatically learn and self-improve.  This is where the Rethink works.  


### AgenticAI Design Patterns {#AgenticAIDesignPatterns}

The 4 agentic ai design patterns(3) are:

Reflection:  This is similar to Rethink.  It is here that the agent can self-correct its errors, make intelligent decisions and adapt based on the updated knowledge
Tool Use: Access to the tools make the agent use external sources to garner information that it will not be able to do on its own.  This is important as it allows the agent to initiate actions that improve its decision making process
Planning: This is where the task decomposition and broken down into further subtasks based on the goal.  Strategies are formulated here to make those autonomous decisions.
Multi-Agent :  The power of agentic AI lies in the ability to have multiple agents work in collaborative, hierarchical, competitive or in a mixed format to achieve the objectives within the constraints defined in the goals.

![AgenticAI](/assets/images/intro_strategy/media/AgenticAIPatterns.png)

Figure 2:  The 4 agentic ai design patterns[6]

There is a similarity in the architecture of agentic ai with that of organizational behaviour.  In organization, the triad of People-Process-Technology is aligned with the Value Proposition or the Goals of the Company.  The goals of the company is what drives the mission. The hierarchical nature of the organization which contains the capabilities on which the organization functions.  This is the people aspect of the business.  This constitutes the ‘WHO’ or the culture of the organization. The process is the governance or ‘HOW’ it operates. The roles & responsibilities drive the ‘WHAT’ of the operation.  This constitutes the technology. Network dependent competencies can also be incorporated in MAS. Think of this as the skill-set matrix that is commonly employed in organizations to identify the strength in the skills of the organization and any gaps that requires upskilling or reskilling. The value proposition tells us ‘WHY’ we are doing this. This is demonstrated in the top portion of Figure 3.


![AgenticAI](/assets/images/intro_strategy/media/HR_OB.png)


![AgenticAI](/assets/images/intro_strategy/media/AgenticAI_CognitionModules.png)

Figure 3. The mapping of the Goals-Capabilities-Resources to Cognitive-( Perception + Cognitive)-Action modules in agentic AI

The lower half of Figure 3 are the modules of Agentic AI : Cognitive, Perception + Cognitive and Action. The Cognitive module constitutes the Goals which states what the objectives of the Agents are. This is the brain which makes the strategies depending on the constraints and the successes that are required to be achieved. The capabilities map to Perception and Cognition module or what skills are required. This is where it perceives the environment like reading the input data and makes decisions and plans to conduct any kind of ‘reflection’ that makes the agents autonomous.  The agents need to take Action by accessing LLMs, memory, compute resources and persistent storage.  There are the technological or infrastructure assets as shown in Figure 4.

![AgenticAI](/assets/images/intro_strategy/media/GoalsAgenticAINodes.png)

Figure 4. The mapping of the People-Process-Technology and the corresponding Autonomy &Reasoning, Control layer and Agents & Tools.

The edge between Cognition and Perception + Cognition is Autonomy & Reasoning, the WHO aspect of Agentic AI.  The edge between Cognition and Action is the Control layer.  This is the governance or the OS (operating System) of Agentic AI.  Finally the edge between Perception + Cognition and Action is the Agents & Tools.

## Agentic AI Framework using CrewAI {#AgenticFramework}

The framework for the CrewAI is simple and I find it easy to grasp[1,2]. It essentially contains the following foundational elements:
Agent:  This is an LLM-powered unit where there is a clear, division of labour based on the role assigned to each agent which also has a goal. The other component is backstory which gives the context.

This is shown in the following figure:

![AgenticAI](/assets/images/intro_strategy/media/ConfigAgentsRole.png)

Figure 5: The configuration of the agents and the corresponding role, goal and backstory

The summary_agent role here is to summarize the blog (3). The name of the role is “ Summary Specialist with Introspection”. The Crewai document suggests that the name of the role be as specific as possible. 

***Note***:  *Here I want the agent to reflect on itself and hence the Introspection.*

The goal together with the backstory makes up the system prompt.  The goal tells the agent the strategy: the purpose it is to serve.  In this case it is to “Create comprehensive summaries with transparent synthesis process”. 
The backstory captures the expertise, the persona and any constraints that the agent needs to abide by.  Let’s identify each of the concepts based on the colour coded sections in the following backstory:

“Expert at distilling complex information while clearly showing how insights were synthesized from multiple sources”
The constraints (what the agent must follow) ensure that the conditions are fulfilled or satisfied– it’s a must-have.  The persona  guides the behaviour of the agent and how the agent thinks while expertise drives what things the agent can do.

***Note***:  *The LLM used is opensource running Ollama[4] on a local machine and can use a CPU. The LLM used is: llama3.2:1b. You can download Ollama and then pull the appropriate language model using the command: ollama pull llama3.2:1b once the server is running.  To find the list of models that have been downloaded use the command shown in the figure below.*

![AgenticAI](/assets/images/intro_strategy/media/Ollama_models.png)

Figure 6. List of models currently running in Ollama
  
Task:  The Agent calls to complete a specific task.  The task defines the action the agent needs to conduct. The description of the task contains the user prompts. In this case, it is “Create two essential outputs for the blog:” [and the blog content] for the summary_task.

![AgenticAI](/assets/images/intro_strategy/media/ConfigAgentsSummaryTask.png)

Figure 7. The summary_task defines the actions that the agent needs to follow for summary_agent

![AgenticAI](/assets/images/intro_strategy/media/ConfigAgentsQualityTask.png)

Figure 8. The quality_task for the quality_agent.

In addition, the context in which order the agents are to run are also included.  The output of the previous agent’s task is included in the context. The summary_task action is carried out by the summary_agent.  In essence, the context parameter contains all the dependencies of the task.
The output of the summary is then structured in 3 parts consisting of a comprehensive summary, the synthesis process and the editorial decisions showing how it made the decision.  This is critical as it brings transparency and as a part of responsible ai you can see the transparency and hence being trustworthy.

***Tip***: *It is better to work on the task first and then craft the agents as the latter is assigned to the tasks. So, a clear enunciation of the tasks makes it easy to assign them to the agents.*

Crew: This is essentially a container with all the agents. Here it is the conductor that orchestrates all the multiple agents to perform the tasks.  The 4 agents, Research, Script Writer and Summary, which are the worker bees are asked to perform sequentially.  The main.py file acts as the main coordinator which then calls the worker_orchestrator.py file that then calls the introspective_orchestrator.py  The framework itself uses a process to coordinate the agents which can run sequentially, in parallel or a conjunction of both. This is done by calling the Process.sequential enumerator. 

***Note***:  *In case of the CrewAi framework there is additional Coordinator module that orchestrates implicitly the agents*

***Note***: *According to the documentation[4], “Processes orchestrate the execution of tasks by agents, akin to project management in human teams. These processes ensure tasks are distributed and executed efficiently, in alignment with a predefined strategy”.*

Finally the execution is performed by calling the kickoff() function. This is shown in Figure 9.

![AgenticAI](/assets/images/intro_strategy/media/ConfigAgentsCrewKickoff.png)

Figure 9. Crew containing the sequential process of the agents and the execution 

Tools: The tools are used to do a search eg web search, connecting to APIs that allow for seamless integration.

I have used progressive prompt hint to improve the reasoning of LLMs [7].  The agent that checks the quality validates the facts, checks logical consistency and corrects any errors and provides the feedback to improve the process.  There is a learning that happens based on the feedback. So you can see that there is a reflection built in the quality_agent.  This makes this agentic ai system self-learning as it not only evaluates but also learns while it corrects during the process.  The whole gamut of perception, cognition, action and reflection is being performed in the system from the input, to thinking, followed by the actions and finally the reflection. 

***Note***:  *The quality_agent only reads and assess it does not make any feedback loop. The process is marked sequential and there is a simple iteration.*

The architectural diagram is shown in Figure 10.  Please note that within the container the Sequential process is first run followed by the tasks.  Each of the task then calls upon the agents to do their work and uses the LLM.  The input is initially fed to the container and the result from the container is then provided as the output.

![AgenticAI](/assets/images/intro_strategy/media/CrewAIContainer.png)

Figure 10. Architecture of the current setup

The mapping of Cognitive- (Perception+Cognitive)-Action modules with that of the CrewAI framework in shown in figure 11.

![AgenticAI](/assets/images/intro_strategy/media/AgenticAI_CrewAI.png)

Figure 11: The CrewAI components and the associated Classes and functions of the framework
Here is a snippet of the Quality Assurance Validator on executing the main.py file

![AgenticAI](/assets/images/intro_strategy/media/QualityAnswerValidator.png)

Figure 12. Quality Assurance Validator

Since the confidence was low based on the quality the system was not able to provide the report.  The main consideration over here is that the quality agent was doing a sequential process with a single iteration.  A feedback loop where there is a supervisor agent that coordinates the iterations of the agents and then based on the quality of the scores makes conditional executions which then feeds back to the agents need to be considered to increase the service. 

I tried with another agentic ai system that did not incorporate introspection, progressive-hint prompting and the quality agent and it provide the summary unlike the previous case.  Here is a snippet of the summary report.

![AgenticAI](/assets/images/intro_strategy/media/SummaryAssessmentPart1.png)

Figure 13.  Summary report of the blog without the quality agent and introspection.

The main consideration of the summary report with 2 distinct cases that demonstrate the power of reflection in the system.

## 🔗 Code Repository

The complete code and analysis tool is available in Github.

REFERENCES

1\.	https://deepwiki.com/crewAIInc/crewAI/1.3-key-concepts

2\.	https://github.com/crewAIInc/crewAI

3\.	https://sujpaul.github.io/ai/strategy/ml/dl/Exploring-Current-Internal-and-External-Environment/names of the agents

4\.	https://ollama.com/download

5\.	Ranjan Sapokta, Konstantinos I.Roumeliotos, Manoj Karkee, “AI Agents vs Agentic AI: Conceptual taxonomy, Applications and Challenges”, Elsevier, August 2025

6\.	https://www.analyticsvidhya.com/blog/2024/10/agentic-design-patterns/

7\.	Chuanyang Zheng, Zhengying Liu, Enze Xie, Zhenguo Li, Yu Li, “Progressive-hint Prompting Improves Reasoning in Large Language Models”, https://arxiv.org/abs/2304.09797

