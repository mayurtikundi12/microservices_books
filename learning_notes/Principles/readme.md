SOFTWARE DEVELOPMENT PRINCIPLES
-----------------------------------

@link: https://enterprisecraftsmanship.com/posts/most-valuable-software-development-principles/

These principles make our code live long and happy.
Extensible
Maintainable
 
1. YAGNI    [ You Ain't Gonna Need It ]  => Don't keep unwanted code
2. KISS    []   => Keep code simple
3. Fail Fast principle





BEST PRACTICES:

1. Make sure you don’t expose the internals of your code base and properly encapsulate your entities.

2. Try to achieve low coupling and high cohesion in your code base on each level. Don’t fall into the trap of destructive decoupling, through. In most cases, it is as harmful as Big Ball of Mud.

3. Don’t repeat yourself, but at the same time, don’t confuse the DRY principle with code duplication. Remember, this principle is about domain knowledge, not the text on the screen.

4. Let your application fail fast. Always strive to shorten the feedback loop even if it means your software will feel less stable. With this technique in hand, such situation won’t last long anyway.

5. Try to always make your assumptions explicit in code. Agree upon conventions clearly, don’t allow misunderstanding affect your performance.