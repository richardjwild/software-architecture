[Software Architecture](..) > Patterns

---

# Software architecture patterns

Architectural designs in software do not need to be invented from scratch for every system. There are by now a number of different architectural patterns that are widely known. These patterns are similar in concept to the better known [Gang of Four design patterns](https://springframework.guru/gang-of-four-design-patterns/), in that they are generalised designs which can be applied to software systems to solve common classes of programming problems. The difference is that the Gang of Four-style design patterns are intended to be implemented in object-oriented programming languages in particular. Architectural patterns are not OO designs: they can be implemented in almost any programming language. Also, the GoF patterns are solutions to very specific programming problems; they are just not *domain* specific. The types of problem that architectural patterns solve are more general. Moreover, they lend shape to the whole system: a system cannot be refactored away from an architectural pattern without substantially re-implementing it.

Unlike the GoF design patterns, which were carefully curated and presented in the book of the same name, there has been no attempt as far as I know to do anything similar for architectural patterns. Although most of these patterns are widely known, individuals' knowledge is usually quite patchy: the average software engineer can typically name a few patterns. A software engineer who can discuss many different architectural patterns and elucidate the types of problem each is well suited for is quite rare. Unfortunately, when software engineers are called on to make architectural decisions, their choices are based all too often on what is fashionable at the time, rather than by an objective analysis of the problem and a consideration of the architectural patterns and their respective suitability.

This is what I am trying to address here. I am not aware of any serious study of architectural patterns that has systematically collated them, and presented them together with the particular aspects of the problem domain that indicate (or otherwise) the appropriateness of each pattern. I am attempting to fill that gap. It should not need to be said (but I shall anyway) that this is most assuredly not a complete list of the architectural patterns that are known, it is merely the ones known to me. And the criterion that makes a design pattern architectural is still rather woolly: I contend that software design becomes architecture when it is difficult to change, but there are degrees of difficulty. Precisely *how* difficult (or how to measure that) I have left unanswered. Even if it were possible to compile a complete list, it would still only be accurate at the time of writing. More architectural patterns will surely be discovered in the future.

As for the categorisation, that is entirely my own work. I have grouped the architectural patterns covered here into six separate categories:

![Architectural patterns grouped into categories.](software-architecture-patterns.jpg)

Some of these patterns preclude the use of others, for example monoliths and microservices are generally defined in opposition to each other. There are nonetheless many more acceptable combinations than there are incompatible ones. For example, there is nothing to stop you using the CQRS pattern in a monolithic application that employs a hexagonal architecture, or a microservice that is implemented as an n-tier application.

Wherever possible the patterns are described in technology-agnostic terms, even in the cases where common products exist that are famously associated with the pattern. I believe that technologies come and go more rapidly than design and architecture patterns do, and it is my hope that by not tying this guide to specific technologies it will remain relevant for longer. There are some exceptions: the web application architectural patterns seemed important enough to include, and it is impossible to discuss those without making reference to HTTP, etc. Similarly, it is not really feasible to discuss resource-oriented API designs without talking about REST and HATEOAS, even though they too are intrinsically associated with HTTP.

## No architecture at all

The [big ball of mud](big-ball-of-mud) is not in any category because it is not an architectural pattern. It is, rather, the complete absence of architecture in a software system. It deserves mentioning because it could still be argued to be an architectural style, and it is also very common out in the wild, probably more so than we care to admit. It has many severe drawbacks but it is nonetheless not wholly without virtue, and it is instructive to know the forces that drive software systems into this state.

## Architecture Patterns

| [Code design](code-design) | These patterns pertain to the structuring or organisation of the code internally within an application. |
| [System Distribution](system-distribution) | These patterns describe methods of organising systems that are distributed across multiple computers. |
| [Messaging](messaging) | These patterns pertain to the flow of control through a system via messages or events. |
| [Web Applications](web-applications) | These are patterns of structuring and distributing web applications. |
| [API Design](api-design) | Patterns of designing remote APIs. |
| [Data Organisation](data-organisation) | These are patterns of organising and structuring data in a persistent store. |
