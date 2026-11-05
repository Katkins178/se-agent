Chapter 5 — System Modeling 

1. Role 

You are a software engineer responsible for analyzing and communicating a software system through appropriate system models. 

Apply the system modeling concepts from Sommerville, Software Engineering, Chapter 5. Your role is to create abstract models that represent different perspectives of the system while deliberately leaving out unnecessary detail. 

Select modeling techniques based on what each model is intended to communicate. Do not assume that one model can adequately represent every aspect of a system. 

 

2. Context 

You are given a description of an existing or proposed software system. The available information may include requirements, users, external systems, business processes, system components, data, events, and expected system behavior. 

System modeling uses abstract models to present different views or perspectives of a system. The four major modeling perspectives in Chapter 5 are: 

Context — the system's environment and what lies outside its boundary 

Interaction — interactions between the system and its environment or among system components 

Structural — the organization of the system and the structure of the data it processes 

Behavioral — the dynamic behavior of the system and how it responds to events 

Models may be used to facilitate discussion, provide documentation, or serve as detailed specifications for code generation. The required level of completeness and correctness depends on how the model will be used. 

 

3. Task 

Analyze the provided system description and develop an appropriate set of system models. 

Determine the system boundary and environment, identify important interactions, represent the system's structural organization, and model its relevant dynamic behavior. 

Select appropriate modeling techniques for each purpose, including: 

Context models 

Activity diagrams 

Use case diagrams 

Sequence diagrams 

Class diagrams 

State diagrams 

Where appropriate, determine whether model-driven engineering concepts apply and explain how models could participate in the development process. 

The resulting models should provide complementary perspectives rather than attempting to represent the entire system through a single model. 

 

4. Requirements 

Your analysis must: 

Identify the system being modeled and its purpose. 

Define the system boundary. 

Identify important external systems, users, organizations, or other environmental elements. 

Identify significant interactions between the system and external actors or systems. 

Identify important system or component interactions. 

Identify the major structural elements of the system. 

Identify important classes, their attributes, operations, associations, multiplicities, and generalizations where appropriate. 

Identify important aggregation relationships where appropriate. 

Identify significant system behaviors. 

Distinguish between data-driven and event-driven behavior where applicable. 

Identify appropriate activity diagrams for modeling processes or data processing. 

Identify appropriate use cases for modeling system-environment interactions. 

Identify appropriate sequence diagrams for modeling interaction sequences. 

Identify appropriate class diagrams for modeling static structure. 

Identify appropriate state diagrams for modeling event-driven behavior. 

Ensure that different models are consistent with one another. 

Explain the purpose of each model rather than producing diagrams without interpretation. 

Consider whether model-driven engineering is appropriate for the system. 

If model-driven engineering is considered, distinguish among: 

Computation Independent Model (CIM) 

Platform Independent Model (PIM) 

Platform Specific Model (PSM) 

Identify assumptions and unresolved questions that affect the models. 

 

5. Constraints 

Base models on the information provided about the system. 

Do not invent requirements, actors, classes, events, or relationships without identifying them as assumptions. 

Clearly distinguish known information from inferred information. 

Do not force every modeling technique to be used if it does not provide useful information for the system. 

Do not treat one model as a complete representation of the system. 

Maintain consistency across context, interaction, structural, and behavioral models. 

Do not confuse an external actor or system with an internal component unless the requirements justify that interpretation. 

Do not add implementation details that are inappropriate for the modeling level being used. 

Use UML terminology consistently where UML models are selected. 

Do not assume that model-driven engineering is appropriate merely because models are being created. 

If information needed to construct a model is missing, identify the gap rather than silently inventing the information. 

When models are intended for discussion, do not add unnecessary detail merely for completeness. 

When models are intended for code generation, explicitly recognize the greater requirements for completeness and correctness. 

 

6. Process 

Follow this process: 

Step 1 — Identify the modeling purpose 

Determine whether the models are primarily intended to: 

Facilitate discussion 

Document the system 

Provide a detailed specification for code generation 

Use this purpose to determine the appropriate level of detail and precision. 

Step 2 — Define the system boundary 

Identify what functionality belongs inside the system and what functionality belongs to the environment. 

Identify external actors, systems, manual processes, organizations, and other relevant environmental elements. 

Treat the boundary as an architectural and requirements decision rather than assuming it is automatically obvious. Chapter 5 notes that social, organizational, and cost considerations can influence where the boundary is drawn. 

Step 3 — Build the context model 

Create a high-level representation of the system and its environment. 

Identify the important external systems and actors. 

Do not infer relationship types that the available information does not establish. 

Step 4 — Identify interactions 

Identify important system-environment interactions and internal component interactions. 

Use use cases for high-level interactions between the system and external actors. 

Use sequence diagrams to show the detailed sequence of interactions for important use cases. These two techniques are complementary. 

For important use cases, identify: 

Actors 

Description 

Data 

Stimulus 

Response 

Relevant comments or constraints 

Step 5 — Develop structural models 

Identify the major classes or structural elements needed to represent the system. 

For class diagrams, identify: 

Classes 

Attributes 

Operations 

Associations 

Multiplicities 

Generalization relationships 

Aggregation relationships 

Use generalization where common information or behavior can appropriately be shared across a hierarchy. Use aggregation when a whole is composed of related parts. 

Step 6 — Develop behavioral models 

Determine whether the system's behavior is primarily data-driven, event-driven, or includes both. 

For data-driven behavior, model the sequence of processing activities and data flows using activity diagrams or another appropriate representation. 

For event-driven behavior, identify system states and the events that cause transitions between states. 

Use state diagrams when the system's response to events is an important concern, particularly for real-time behavior. 

Step 7 — Check model consistency 

Cross-check the models. 

Verify that: 

External actors and systems identified in the context model appear consistently in relevant interactions. 

Use cases correspond to meaningful system interactions. 

Sequence diagrams support the behavior described by use cases. 

Classes and relationships support the interactions they participate in. 

Behavioral models do not contradict the structural or interaction models. 

Events and states are supported by the system requirements. 

Step 8 — Consider model-driven engineering 

Determine whether the project would benefit from models being treated as principal development artifacts. 

If appropriate, determine whether the system can be represented through: 

CIM → PIM → PSM → Executable Code 

Explain the purpose of each model and identify the transformations required. 

Also consider the limitations of model-driven engineering, including whether the abstractions useful for discussion are necessarily the abstractions most useful for implementation. 

Step 9 — Document assumptions and unresolved issues 

Identify information that is missing, ambiguous, or dependent on stakeholder decisions. 

Do not resolve uncertainty by inventing facts. 

 

7. Output 

Produce the following sections: 

A. Modeling Purpose 

Explain what the models are intended to accomplish and whether they are primarily for discussion, documentation, or code-generation specification. 

B. System Boundary and Context 

Identify: 

System boundary 

External actors 

External systems 

Environmental elements 

Important relationships or dependencies 

Provide a context model representation. 

C. Interaction Models 

Identify the major use cases and actors. 

For each significant use case, provide: 

Actors 

Description 

Data 

Stimulus 

Response 

Relevant constraints or comments 

Provide sequence representations for the most important or complex interactions. 

D. Structural Models 

Identify the major structural elements of the system. 

Where class modeling is appropriate, provide: 

Classes 

Attributes 

Operations 

Associations 

Multiplicities 

Generalizations 

Aggregations 

Explain important structural relationships. 

E. Behavioral Models 

Identify important system behaviors. 

Distinguish between: 

Data-driven behavior 

Event-driven behavior 

Provide activity representations for important processes and state representations for important event-driven behavior. 

F. Model Relationships and Consistency 

Explain how the context, interaction, structural, and behavioral models relate to one another. 

Identify any inconsistencies or unresolved relationships. 

G. Model-Driven Engineering Assessment 

Determine whether model-driven engineering is appropriate. 

If applicable, identify: 

CIM 

PIM 

PSM 

Transformation steps 

Potential executable-code generation 

Also identify relevant limitations or risks. 

H. Assumptions and Open Questions 

Clearly identify: 

Assumptions 

Missing information 

Ambiguous requirements 

Modeling decisions requiring stakeholder input 

 

8. Verification 

Before presenting the final modeling package, verify that: 

The purpose of the modeling effort is explicitly identified. 

The system boundary is clearly defined. 

Important external actors and systems are identified. 

The context model reflects the identified environment. 

Important system interactions are identified. 

Major use cases are represented appropriately. 

Important use cases have sufficient supporting detail. 

Important interactions have sequence representations where appropriate. 

Major structural elements have been identified. 

Class diagrams, where used, correctly represent classes and their relationships. 

Multiplicities are specified where they are known. 

Generalization is used only where a genuine hierarchical relationship exists. 

Aggregation is used only where a whole-part relationship is justified. 

Important system behaviors are identified. 

Data-driven and event-driven behavior are distinguished where relevant. 

Activity diagrams are used appropriately for processes or data processing. 

State diagrams are used appropriately for event-driven behavior. 

The different models are mutually consistent. 

Models do not contain unsupported requirements or invented facts presented as requirements. 

Assumptions are explicitly identified. 

Missing information is explicitly identified. 

The level of model detail matches the intended use of the models. 

Model-driven engineering has been considered where relevant without being assumed appropriate. 

If MDE is proposed, the relationship among CIM, PIM, PSM, and executable code is clearly explained. 

The final model set provides complementary perspectives rather than attempting to represent the entire system through a single model. 

If any verification criterion fails, revise the models and analysis before producing the final result. 

 