---
title: "Ontology creation : mapping of AgenticAI CrewAI Framework"
date: 2025-12-17
categories: [AgenticAI, CrewAI, Ontology, Protege, Equivalence, Constraints]
tags: [AgentAI, LLM,AgencticAI, CrewAI, Ontology, Protege, Properties, Axioms, Concepts]
read_time: true          # Shows estimated reading time (e.g., "7 min read")
toc: true                # Enables Table of Contents
toc_sticky: true         # Keeps TOC visible as you scroll (nice for long posts)
comments: false
---

## Introduction

In this blog I will demonstrate the purpose behind the usage of ontologies as the foundational stone for building AgenticAI.  Using the earlier blog of creating a summary report using the CrewAI framework, I will build an ontology that maps to the framework.  This can then later be used to build the code for the summary report.  

## Ontology useage in knowledge representation

Gruber[1] described ontology as a formal explicit specification of a shared conceptualization. “Formal explicit specification” describes the concepts, properties and the relations that exist between them that can be represented in formal languages like RDF/RDFS and OWL.  This allows the concept to be arranged in hierarchical manner.   “Conceptualization” refers to the knowledge domain that exists in the organization while “shared” means the existence of both tacit and explicit knowledge.
Organizational behavioural and operation management are replete with studies on how to harness both explicit and tacit knowledge to foster and drive innovation. Explicit knowledge is represented in words, drawings, documents and other blueprints that can be communicated to others[2]. On the other hand, tacit knowledge is invisible.  It is something that both individuals and organizations develop, retain and accrue over the years through formal and informal means of learning that differentiates the competitiveness of the organization.  This knowledge resides inside the head of each individual and with organizational churning or people moving out to other department also carries with it this tacit knowledge.  It is therefore important to capture this knowledge and convert into explicit knowledge that gives the competitive edge.  This is where knowledge engineers tap into the domain expertise withing the organization to develop the ontology that encompasses both tacit and explicit knowledge along with all the structured and unstructured data.  The semantics of ontology provides a common vocabulary and a reasoning power[3] that can be communicated across the organization. 
Knowledge includes concepts, attributes, axioms and rules that ontology also provides.  Knowledge acquisition is therefore hierarchical and also an incremental process. Eliciting this intellectual capital that resides with domain expert and marshalling into a knowledge based becomes a strategic imperative for companies trying to seek competitive advantage.

A knowledgebase[4] can be defined in a 4-tuple format:

KB = (O,I,inst,instr)   …..  (1) 


Where
KB= knowledgebase
O= ontology
I = instances
Inst = function; also called concept instantiation
Instr= function; also called relation instantiation
The conceptualization of knowledge can therefore be facilitated by the creation of ontology. This is represented in a 5-tuple structure[4]

O:=(C,R,HC,rel,A)    …. (2)

Where 
C, R: Concept and relation identifiers
HC: directed, hierarchical concept such that HC(C1, C2) states that C1 is a subconcept of C2
Function rel: relation which identifies concept as the domain and the range of the relation is identified by data types
A: represents the set of axioms
The representation between knowledgebase and ontology is shown in Figure 1

![Ontology](/assets/images/intro_strategy/media/kb_onto.png)

Figure 1 Representation between knowledgebase and ontology(the diagram has been generated

***Note***: *As we develop the ontology you will see that ontology is created based on language based axioms that needs to be formalised.  It’s based on an open-ended view of the world where everything is allowed till you place restrictions and constraints in the development*

Ontology therefore provides a structured format to represent the knowledge.
Based on equation 1, an ontology consists of concepts.  Classes represent concepts that are in the domain[6].  Classes have instances similar to the instances in object-oriented programming programs(OOPs).  As with OOPs, an instance is a child of the Class that can be identified as ‘is-a’ relationship and also inherits the Properties which can be regarded ‘part-of’.  Although, object-modeling of ontology might sound similar to OOP, the differences between the 2 are listed below:
CLASSES:
Ontology: Also known as concepts; used for classification.  The purpose is for logical categorization which is the main difference with OOP.  Instances or individuals can inherit classes.
OOP: They also define categories of objects which are instances of classes
PROPERTIES
Ontology: They are first-class-citizens.  They act as independent entities with their own logic and can also have sub-properties which facilitates inheritance of properties but not from classes. There are 2 kinds of properties: Object and Data. The former establishes binary relationships between 2 instances and Data properties link to literals.  
OOP: The attributes in classes are regarded as properties and hence unlike ontology is owned by the classes.
INSTANCES
Ontology: Specific members of a class.  However, unlike OOP ontology can infer whether an instance belongs to a class by reasoning through the properties.
OOP: Similar to the ontology where an object is an instance of a class.
INHERITANCE
Ontology: SubClassof a class and supports multiple inheritance.  Ontology inheritance facilitates reasoning due to set inclusion and is used for logical reasoning unlike OOP.  
OOP: Objects created from the class inherits both the attributes and methods of the class.  There is no reasoning.  The developer has to build in logic in the program.
AXIOMS & FUNCTIONS:
Ontology: Axioms are logical constraints.  They are declarative constraints what must be true are declared. Functions are not a standard OWL construct
OOP: Methods and functions define the behaviour of objects and are executable code and unlike Ontology states how to do things.
OPEN-WORLD ASSUMPTION(OWA) vs CLOSE-WORLD ASSUMPTION(CWA)
Ontology: Ontology is OW. If a fact is not stated or inferred that means it is unknown.  It does not mean false This means it allows for non-monotonic reasoning (NMR) by allowing conclusions later to be adjusted should new facts arrive.  This makes it more flexible and robust.  
OOP: This only allows CWA.  So if a fact in not present in the program or database it is considered false.
REASONER:
Ontology:  it can classify individuals, infer new class memberships and check for ontology consistency.  Relationships are explicitly defined. Reasoning by deduction is automatic
OOP:  programmers has to manually enter the logic in the code. Reasoning has to be built-in by the programmer.


### Creating the Ontology using Protégé

Protégé is an open source tool that can be downloaded from protégé.stanford.edu.  I have used it in the past before and have found the instructions for the installation simple to use.  It has a very good tutorial that is easy to pick up the basics.  Here is the link to the tutorial[5].
Since the code for the AgenticAI using CrewAI have already been written I will show the reverse way of creating the ontology and mapping to the code.  The original python code using CrewAI is available at the github site.  
Everything in Protégé is inherited from owl:Thing.  The classes or concepts that are created are inherited from this so it is easier to categorize the difference concepts.  Both classes and concepts are interchangeably used in this article. This can be seen on the left side of the panel in Protégé where all the classes are listed as in Figure 2. The mapping of 2 of the classes, Crew and Process as per the code in the file  workflow_executor.py is also shown beside it.


![Ontology](/assets/images/intro_strategy/media/ontoconcepts_mapping.png)

Figure 2:  The ontological concepts for each of the categories shown in Protege

The concepts have been categorised into 3 that are listed as : AIComponent, Content and CrewAgenticAI.  The subclasses for each of the classes are listed below each of the categories.  The AIComponents has LLM as a sub-class and ollama is the instance that is being used in this case.  Likewise, ModelConfig and Prompt are the 2 sub-classes that inherit from AIComponents.  Similarly, Content has 4 sub-classes that are: Analysis, BlogPost, Quality and Summary.  The CrewAI framework in this case has 4 classes that was used: Agent, Crew, Process and Task.  The Process class has 3 classes; HierarchicalProcess, ParallelProcess and SequentialProcess. By looking at the code  in workflow_executor.py , I can see that the Process that I used was sequential as I wanted the Tasks that had 4 instances of researchtask, structuretask, summarytask and qualitytask is assignedto the respective instances of researchagent, structureagent, summaryagent and qualityagent to the Agent class.  This is shown in Figure3 by using OntoGraf in Protégé.


***Note***: *I have checked OntoGraf that comes with the installation of Protege.  Just select Window/Tabs/OntoGraf*

![Ontology] (/assets/images/intro_strategy/media/Ontograf_concepts.png)
Figure 3. Ontograf representation of the Concepts in Protege

The inheritance in blue straight arrows are pointed towards each of the subclasses.  The purple coloured arrows are connected to the nodes contained with diamond-shaped instances of the classes.  By hovering around the arrows between the parent class and the child class it will display in the format: ParentClass – has individual  instance.  For example the arrow between Agent and structureagent it would be represented as Agent – has individual structureagent. The broken arrows in yellow marked between 2 classes as between Agent and LLM is a Property that is being used.  In this case, it is an Object Property which is shown as Agent –usesLLM (Domanin > Range)LLM. 
Note: In OWL ObjectProperties connects to other instances while Dataproperties connects to literal values like strings.  There is also AnnotationProperties which allows you to include any additional metadata to add richness
By right-clicking on the node for Task and then clicking on Show neighbourhood, I can see the following in Figure 4.  I can then add in other nodes and instances to dig deeper into the relationships with Task.

![Ontology](/assets/images/intro_strategy/media/Ontograf_Task.png)

Figure 4. The relationships and the instances of Task and its neighbourhood

From the above figure, summaryAgent is an instance of Agent, which usesLLM and the instance of LLM that it uses is ollamaLLM1.  This, usesLLM, is shown as an ObjectProperty whose domain is Agent and the range is LLM. So all the instances of Agent will make use of this ObjectProperty.  The integration of the ontology layer for  summary_agent as in Figure 4 to the code in introspective_orchestrator.py using the CrewAI framework is shown in Figure 5.

![Ontology](/assets/images/intro_strategy/media/summaryagent_onto.png)

Figure 5. Mapping of summaryAgent to the agenticai code

If I now click on Set as Focus on Task, I can then concentrate on this node and the impact it has on the others.  This is shown in Figure 6.

![Ontology](/assets/images/intro_strategy/media/Onto_Task_focus.png)

Figure 6. Set to focus on the Task node

This helps to concentrate on Task and what the associated classes and properties it is servicing.  The circle attached to the node is a self-loop.  The graph does not tell us that.  By clicking on ObjectProperties for Task and then selecting hasContext, it can be seen that both the Domain and Range refers to Task. This allows iteration, chaining and DAG(directed-acylic-graph) based execution and feedback loop.  However, creating an instance of a self-referencing class does not mean it’s going to inherit them.  The instances of the class, Task,  as in the code(introspective_orchestrator.py): 

context=[self.research_task, self.structure_task, self.summary_task]
merely exhibits dependencies bearing in mind that ontology classes are static structures where execution is not propagated down the chain.  The dependencies are such that the output of one task follows the input of the next task.

In Figure 4, there is a symbol ‘≡’ on the left hand side of Task. 
This is shown in Figure 7.

![Ontology](/assets/images/intro_strategy/media/equivalence_Task_onto.png)

Figure 7. Equivalence of Task

By conditions listed under EquivalentTo are the constrains that are inherited by the sub-classes that instances of these classes must satisfy them.  So these equivalent axioms of Task defines what it is to be a Task.  That means, both the ObjectProperties and the DataProperties listed in Figure 7 defines what it means to be a Task.  These are the necessary and sufficient conditions that each instances of Task will be considered if and only if it satisfies all these conditions.  The reasoner would then infer that it is a Task.  Mathematically, this can be stated as follows:

Task ≡  (assignedTo exactly 1 Agent)
⊓ (hasDescription exactly 1 xsd:string)
⊓ (hasExpectedOutput exactly 1 xsd:string)



***Note***: *‘⊓’ means intersection; can also be regarded as ‘and’*

Here the ObjectProperties are the membership constraints that are inherited by subclasses and enforced by instances.  Constraints as you can see tell us where to apply them and provides guardrails and safety and makes the ontology stronger.  So when the reasoner sees that the researchTask is an instance of Task it ensures that it must have:

exactly assignedTo 1 Agent
exactly hasDescription 1 string
exactly hasExpectedOutput 1 string


If its absent then the ontology will be marked as inconsistent.  So in Figure 8, you can see that the instance, researchTask has indeed satisfied the conditions and have additional ObjectProperties, hasInput and produces.

![Ontology](/assets/images/intro_strategy/media/researchTaskonto.png)

Figure 8. researchTask as an instance of Task showing the constraints


***Tip***:  *This will be marked in red-colour at the bottom of the application beside Show Inferences.  Ensure that you have selected any of the reasoner’s from the Reasoner menu and have started the Reasoner.*

Properties as mentioned earlier are first-class axioms.  This means that both ObjectProperties and DataProperties are independent of each other.  They can have their own axioms, hierarchy, inferences, constraints but are not any attributes of any classes, a key difference with OOP.  They only inherit if they have sub-properties.  For example, an ObjectProperty called stronglydepend  will be a sub-property of depend.  As such, it applies to all Classes and instances and hence it is global. 


***Tip***: If you click on Object-Property in Protégé you will see the list of all ObjectProperties under-owl:TopObjectProperty. You can then select any ObjectProperty and can create a sub-property from the tool menu  

Since Properties are tied to individuals, the relationship in Object Properties are binary and they tie the 2 individuals.  For example, the ObjectProperty usesLLM ties the Agent class to the instance of LLM, ollamaLLM1. This is something I have mentioned earlier.

***Note:***  *Classes classify individual, individuals are related to Properties and constraints with Axioms.  The open-ended reasoning enables OWL language to facilitate classification, inference and knowledge representation as mentioned earlier.)

Figure 9 shows how the instance of researchTask in the ontology created is mapped to the agenticai code(introspection_orechestrator.py) in the previous blog.  

![Ontology](/assets/images/intro_strategy/media/researchtaskonto_mapcrewai.png)

Figure 9: Addition of other guardrails for researchTask in the ontology, marked in black, that were not present in the code. Items marked in red shows the existence in the code that mapped to the ontology.

The extended ontology properties show the additional guardrails that have been added to the ontology for the researchTask instance that are missing in the introspective_orchestrato.py that needs to be added to the code. These properties are marked in black. The Constraint Properties are the ones that must exist for the instance which has been inherited from the class, Task and the properties that are mapped to the agentic ai code are marked in red.
The mapping of each of the instances of Task with the existing agentic ai code of the previous blog are shown in Figures 10, 11 and 12.

![Ontology](/assets/images/intro_strategy/media/equivalence_structureTask_onto.png)

Figure 10. Addition of other guardrails for structureTask in the ontology, marked in black, that were not present in the code. Items marked in red shows the existence in the code that mapped to the ontology.

![Ontology](/assets/images/intro_strategy/media/equivalence_summaryTask_onto.png)

Figure 11. Addition of other guardrails for summaryTask in the ontology, marked in black, that were not present in the code. Items marked in red shows the existence in the code that mapped to the ontology.

![Ontology](/assets/images/intro_strategy/media/equivalence_qualityTask_onto.png)
Figure 12. Addition of other guardrails for qualityTask in the ontology, marked in black, that were not present in the code. Items marked in red shows the existence in the code that mapped to the ontology.


## Conclusions & Future Work{#Conclusions}
In this blog I have demonstrated the power of using ontology that explicitly specifies the shared conceptualization and formalizing axioms.  The use of guard rails through equivalence whereby ObjectProperties and Data properties together constitutes what it means to belong to that class.  I have also shown how Protégé can be used to create an ontology and the difference between ontology and OOP.  I have also mapped out the ontology with the agentic ai code using CrewAI framework in the blog:” Creating a Report Summary with CrewAI- framework for AgenticAI” https://github.com/sujpaul/ai_blogsummary

In the next blog, I will discuss the strategy and the implications of developing an ontology for the usage of LLM.

REFERENCES

1\.	Gruber, T.H., “Towards principles for the design of ontologies used for knowledge sharing”, International journal of Human-Computer Studies, 43(5/6), 2001

2\.	McBriar, I., Smith, C., Bain, G., Magraw, S., Gordon, J.L., Risk, gap and strength: key concepts in knowledge management”, Knowledge-Based systems, 16, 29-36, 2003

3\.	https://pmc.ncbi.nlm.nih.gov/articles/PMC4300097/

4\.	Maedche, A., “Development and Applications of Ontologies”, 12th European Conference on Machine Learning/5th European Conference on Principles and Practice of Knowledge Discovery in Databases, ECML’01/PKDD’01, Freiburg. Germany, 2001.

5\.	https://protege.stanford.edu/publications/ontology_development/ontology101.pdf

6\.	Noy, F, N., McGuinness, D., “Ontology Development 101: A Guide to Creating Your First Ontology”, http://www-ksl.stanford.edu/people/dlm/papers/ontology101/ontology101-noy-mcguinness.html


