#1 [DDD Basics -> what,why,whom]

0. DDD helps reduce confusion between multiple parties in SDLC.

1. DDD is a set of tools which allows for a large complex collaborative project having multiple actors in which a common language(terms) is used to model a real life problem domain to a software domain bounded by the context of its domain.

2. DDD  talks about strategically breaking up of a large complex problem according to its use case in real life and modelling it to a software architecture where multiple types of people are working together for the same cause.

3. DDD is about designing software based on models of the underlying domain. A model acts as a UbiquitousLanguage to help communication between software developers and domain experts. 


Book Points By Vuarn Vernon*******************

Chapter 1: Why and What DDD
----------------------------
1. Strategic Design: Broader Details, segregating domain models using strategic design pattern called as Bounded Contexts, and using Ubiquitous language for domain modelling within an explicitly Bounded Context. using subdomains for legacy and Greenfiels project. Integrating multiple bounded contexts using Context Mapping. Context Maps are relations between Bounded Contexts.

2. Tactical Design: Finer Details, Aggregate pattern and Domain Events.

Chapter 2 Strategic Design with Bounded Contexts and the Ubiquitous Language
----------------------------------------------------------------------------

1. Bounded Context is a semantic contextual boundary. That means inside a Bounded Context each component has a specific meaning and does specific things that is only relatable to that context.


2. In the begining of the process the Bounded Context is the Problem Space and with iterations to solve a problem the Bounded Context transitions into a Solution space.



Chapter 3 Subdomains
---------------------

1. Subdomain is a sub-part of your overall business domain.

2. Subdomains can be used to logically break up
your whole business domain so that you can understand your problem space on a large, complex
project.

3. Three primary types of Subdomains
    1. Core Domain 
    2. Supporting Domain
    3. Generic Domain



Chapter 4 Context Mapping
--------------------------

1. Integration of multiple Bounded Contexts in DDD is known as Context Mapping.

2. Source and Consumer

3. Types of Mapping
    1. Partnership
    2. Shared Kernel
    3. Customer(Downstrean) - Supplier(Upstream)
    4. Conformist
    5. Anticorruption Layer
    6. Open Host Service
    7. Published Language


Chapter 5 Aggregates
--------------------

1. Entity : An Entity models an individual thing. Each Entity has a unique identity in that you can distinguish its individuality from among all other Entities of the same or a different type.

Most of the times Entity will be mutable 



2. Value Object : A Value Object , or simply a Value , models an immutable conceptual whole. Within the model the Value is just that, a value. Unlike an Entity , it does not have a unique identity, and equivalence is determined by comparing the attributes encapsulated by the Value
type. Furthermore, a Value Object is not a thing but is often used to describe, quantify, or
measure an Entity.

3. Aggregate : Collection of entities and value-objects, has a root entity which owns all other elements clustered inside it.

4. choose a name that properly describes the conceptual whole that the Aggregate models.








