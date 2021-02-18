---
layout: post
title: Stupid or Solid? 
subtitle: SOLID vs STUPID methodology
---

After viewing the articles assigned, I have learned about the principles labeled as S.T.U.P.I.D. and S.O.L.I.D. and I'll be reviewing each in detail in this blog post.

First lets start with STUPID, which is essentially everything you should avoid when designing a codebase. The acyronym stands for: 
+ Singleton
+ Tight Coupling
+ Untestability
+ Premature Optimization
+ Indescriptive Naming
+ Duplication

The singleton pattern becomes a problem because programs in a global state are hard to test and hide their dependencies. This could also lead to tight coupling. Tight coupling is a generalization of the singleton issue because each program module relies on each of the other modules heavily. Tightly coupled modules are hard to test. This leads us to untestability. If your testing is hard then you probably did a bad job writing code. 

Premature Optimization is considered an anti pattern because its a lot more complex than it seems. You will most likely create unuseable code that is unreadable. Indescriptive naming is pretty self explanitory, we need descriptive names being humans. Finally duplication code is the final sin. The author suggests you become lazy in the right way. 

Now that we have reviewed what stupid code is, lets examine the principles of solid code!

+ Single Responsibility Principle 
+ Open Closed Principle 
+ Liskov Substitution Principle 
+ interface Segregation Principle 
+ Dependency Inversion Principle 

Lets dive into what these principles actually mean. The single responsibility principle essentially states that all classes should have a single responsibility. If you start writing comments that have exceptions then you've boken this rule. 

The open closed principle states that software should b e open for extension but closed for modification. You should remember to make all member variables private by default. The Liskov Substituion principle states that objects in a program should be replaceable with instances of their substypes without altering the correctedness of the program. 

The interface segregation principle states that many client specific interfaces are better than one general purpose interface. Basically you shouldn't have to impliment methods you dont use. Gives you low compling and high cohesion. High cohesion means to keep similar related things together. Your goal is to keep your components focused and try to minimize any dependencies between them. 

Dependency Inversion Principle has two key points. Abstractions should not depnd upon details and that details should depend upon abstractions. This could be rephrased as, use the same level of abstraction at a given level. 

We have now summarized these two set of principles and a main lesson learned from this article is to avoid tight coupling and keep your modules as independent and focused as possible to avoid other issues down the line. 
