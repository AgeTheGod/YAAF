# YAAF - Yet Another Architecture Framework

So why does the world need yet another architecture framework?

The answer is that it doesn't 

Kevin Smith (the author of PEAF - the Pragmatic Enterprise Architecture Framework) lists over 900 Architecture Frameworks on his website [EA Frameworks](https://www.enterprise-architecture.org/ea-frameworks/) so, although we don;lt need another one, I felt like doing this anyway.

Way back in the 2000's I used to write a quarterly column for TDAN called "_Architecture is Objective, Design is Subjective_" where I would discuss various aspects of (mostly) Application Architecture particularly Data Architecture. 
It's always been my belief that all Application Architecture should be Objective based i.e. there must be a clearly defined reason for doing something with a clearly defined outcome for doing it.

I'm also firmly of the belief that Architecture should be driven by Models i.e. Model Driven Architecture (MDA) so I wanted to create a framework that would help people to think about and define their Application Architectures in an objective, model-driven way.

Finally (and this is important) I'm also as lazy as hell so I wanted to create a framework that would help me to avoid doing unnecessary work by re-using existing models and artifacts wherever possible.

##  The Fundamentals

I did my BSc and MSc way back in the mists of time (the 1980 & 1990's) when most application deverkopment was focussed on structured sysrems analysis and the so-called waterfall methodology.

However, things evolve and over the years I've picked up various other ideas and concepts that I think are important to include in any Architecture Framework so here are some of the key ones:

|Term|Abbreviation|Definition|
|----|------------|----------|
|Business Information Model|BIM|A high-level conceptual model that defines the key business entities, their attributes, and relationships within a specific domain or organization. The BIM serves as a bridge between business stakeholders and technical teams, providing a common understanding of the data requirements and structure needed to support business processes and objectives.|
|Domain Driven Design|DDD|An approach to software development that emphasizes the importance of understanding and modeling the core business domain. DDD encourages collaboration between domain experts and developers to create a shared language and a rich model that accurately reflects the business processes and rules. This model is then used to guide the design and implementation of software systems, ensuring that they align closely with business needs.|
|C4 Model|C4|A hierarchical approach to visualizing software architecture, consisting of four levels of abstraction: Context, Container, Component, and Code. The C4 Model provides a clear and structured way to communicate the architecture of a software system to different stakeholders, from high-level overviews to detailed technical designs.|
|Model Driven Engineering|MDE|A software development approach that focuses on creating and exploiting domain models as primary artifacts in the development process. MDE emphasizes the use of models to generate code, documentation, and other artifacts, allowing for higher levels of abstraction and automation. This approach aims to improve productivity, maintainability, and alignment with business requirements by reducing manual coding and promoting model consistency.|
|Consumer Driven Contracts|CDC|A design approach that focuses on defining and managing the interactions between services or components based on the needs and expectations of the consumers (clients) of those services. CDC emphasizes the importance of clear and explicit contracts that specify the behavior, data formats, and communication protocols required by consumers, allowing for better decoupling, flexibility, and evolution of services over time.|

##  The Pillars (or P's) of Architecture

The YAAF framework is based on the 4P's of Architecture:
-  **Perspectives** - Different views of the architecture from different stakeholder roles
-  **Products** - Different types of artifacts and deliverables produced during the architecture process
-  **Processes** - Different activities and tasks performed during the architecture process
-  **Patterns** - Reusable solutions to common architecture problems
-  **Principles** - Guiding rules and best practices for architecture development
-  **Practices** - Established methods and techniques for architecture development

There are other P's that could be included e.g. Plans, Phases, People, Platforms, etc. but I think the above are the most important ones to focus on when defining an architecture framework. Plans and Phases in particular are really Project Management topics and dictated by the development approach being taken.
Platforms are of course important but they tend to be more relevant at the Technical Architecture level rather than the Application Architecture level and do not (or should not) change what an application does and the outcomes it produces.

## Perspectives - Zachman Framework

The [Zachman Framework](https://zachman-feac.com/zachman/about-the-zachman-framework) is one of the most widely recognized enterprise architecture frameworks. It provides a structured way of viewing and defining an enterprise from different perspectives and aspects i.e. it's an Ontology for classifying Artefacts that are created and maintained during the lifecycle of an Organization, Application or System. 

| Perspective (Role)          |               What |                 How |                Where |                      Who |               When |                      Why |
|-----------------------------|-------------------:|--------------------:|---------------------:|-------------------------:|-------------------:|-------------------------:|
| Contextual (Identification) |     Inventory list |     Major processes |        Locations map |                Org units |     Business cycle |           Business goals |
| Conceptual (Definition)     |  Business entities |        Value chains |           Site model |         Stakeholder list |        Event model |      Business objectives |
| Logical (Representation)    | Logical data model |       Process flows |   Distribution model | Roles & responsibilities |       Timing rules |           Business rules |
| Physical (Specification)    |    Physical schema |  Application design |     Network topology |            System owners |          Schedules | Implementation rationale |
| Detailed (Configuration)    |  Table definitions |        Code modules | Deployment artifacts |     Component interfaces | Transaction timing |        Detailed policies |
| Functioning (Instantiation) |       Runtime data | Executing processes |     Production sites |             Active users |   Operational logs |        Measured outcomes |

### Products - Architecture Artifacts

Different types of artifacts and deliverables produced during the architecture process

This is the purpose of a Meta-Model - to define the types of artifacts and deliverables that are produced during the architecture process and the significant details we need to captute about those artifacts in order to manage them effectively.

### Processes

Different activities and tasks performed during the architecture process

### Patterns 

Reusable solutions to common architectural problems

### Principles 

Guiding rules and best practices for architecture development

### Practices 

Established methods and techniques for architecture development
