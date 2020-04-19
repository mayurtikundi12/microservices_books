@link: https://enterprisecraftsmanship.com/posts/dry-revisited/


*KEY POINTS
----------------------------------
1. DRY stands for [ Don't Repeat Yourself ]

2. The DRY principle states that every piece of knowledge must have a single, unambiguous, authoritative representation within a system.

3. The DRY principle restricts the presence of domain knowledge, it doesn’t put any bounds on the actual code which is required to express that knowledge.

4. Comapare the raw code on the basis of the domain it is being used for, it is a bad practice to introduce a base class if the entities do not share the same domain. Hence code duplication of entities having different domains does not violate the DRY principle.