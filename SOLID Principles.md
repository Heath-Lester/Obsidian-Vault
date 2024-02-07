https://en.wikipedia.org/wiki/SOLID
**SOLID** is a [mnemonic](https://en.wikipedia.org/wiki/Mnemonic "Mnemonic") [acronym](https://en.wikipedia.org/wiki/Acronym "Acronym") for five design principles intended to make [object-oriented](https://en.wikipedia.org/wiki/Object-oriented "Object-oriented") designs more understandable, flexible, and [maintainable](https://en.wikipedia.org/wiki/Software_maintenance "Software maintenance"). The principles are a subset of many principles promoted by American software engineer and instructor [Robert C. Martin](https://en.wikipedia.org/wiki/Robert_C._Martin "Robert C. Martin") first introduced in his 2000 paper _Design Principles and Design Patterns_ discussing [software rot](https://en.wikipedia.org/wiki/Software_rot "Software rot")

https://www.digitalocean.com/community/conceptual-articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design

1. Single Responsibility 
	- `A class should have one and only one reason to change, meaning that a class should have only one job.`
	- A class should only have one job
2. Open/Closed 
	- `Objects or entities should be open for extension but closed for modification.`
	- Classes should be extendable without modifying the class itself
3. Liskov Substitution 
	- `Let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a sub-type of T.`
	- Sub-classes (mainly interfaces) should be substitutable for their base or parent class
4. Interface Segregation 
	- `A client should never be forced to implement an interface that it doesn’t use, or clients shouldn’t be forced to depend on methods they do not use.`
	- Split large interfaces into smaller, more specific interfaces
5. Dependency Inversion
	- `Entities must depend on abstractions, not on concretions. It states that the high-level module must not depend on the low-level module, but they should depend on abstractions.`
	- Decoupling by allowing dependencies or inputs to be injected

The SOLID principles have become controversial in the eyes of many who see issues or flaws with object oriented design. In particular with the over-reliance on abstraction. I think like most things, strict adherence to ideological concepts is almost never a good long term strategy.  