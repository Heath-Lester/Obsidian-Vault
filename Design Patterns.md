Refactoring Guru:
https://refactoring.guru/design-patterns
Design Patterns In Use:
https://github.com/milanm/DesignPatternsInUse


Design patterns generally fall into three categories: creation, structural, and behavioral.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/ZfG8BSTX0Lw?si=fMoJSp0YDkPStCET" title="YouTube video player" frameborder="1px" style="border-radius: 4px" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
## Creational Patterns

https://refactoring.guru/design-patterns/creational-patterns

Creational patterns are patterns that include object creation mechanisms. It is said they increase flexibility and re-use of existing code.

1. Factory Method/Virtual Constructor
	- Provides an interface for creating objects in a superclass, but allows subclasses to alter the type of objects that will be created.
2. Builder
	- Constructs complex objects step by step. The pattern allows you to produce different types and representations of an object using the same construction code.
3. Singleton
	-  Ensures that a class has only one instance, while providing a global access point to this instance.
4. Abstract Factory
	- Produces families of related objects without specifying their concrete classes.
5. Prototype/Clone
	- Copies existing objects without making your code dependent on their classes.

## Structural Patterns

https://refactoring.guru/design-patterns/structural-patterns

Structural patterns are patterns that explain how to assemble object and classes into larger structures while keeping structures flexible and efficient.

1. Adaptor/Wrapper
	- Allows objects with incompatible interfaces to collaborate by creating classes that inherit from multiple classes
2.  Bridge
	-  Splits a large classes or a set of closely related classes into two separate hierarchies—abstraction and implementation—which can be developed independently of each other.
3. Composite/Object Tree
	- Composes objects into tree structures and then work with these structures as if they were individual objects.
4. Decorator/Wrapper
	- Attaches new behaviors to objects by placing these objects inside special wrapper objects that contain the behaviors.
5. Facade
	-  Provides a simplified interface to a library, a framework, or any other complex set of classes.
6. Flyweight/Cache
	- Fits more objects into the available amount of RAM by sharing common parts of state between multiple objects instead of keeping all of the data in each object.
7. Proxy
	- Provides a substitute or placeholder for another object. A proxy controls access to the original object, allowing you to perform something either before or after the request gets through to the original object.
## Behavioral Patterns

https://refactoring.guru/design-patterns/behavioral-patterns

Behavioral Patterns are patterns concerned with algorithms and the assignment of responsibilities between objects.

1. Chain of Responsibility
	- Passes requests along a chain of handlers. Upon receiving a request, each handler decides either to process the request or to pass it to the next handler in the chain.
2. Command/Action/Transaction
	- Turns a request into a stand-alone object that contains all information about the request. This transformation lets you pass requests as a method arguments, delay or queue a request’s execution, and support undoable operations.
3. Iterator
	- Traverses elements of a collection without exposing its underlying representation (list, stack, tree, etc.).
4. Mediator/Intermediary/Controller
	- Reduces chaotic dependencies between objects. The pattern restricts direct communications between the objects and forces them to collaborate only via a mediator object.
5. Memento/Snapshot
	- Save and restore the previous state of an object without revealing the details of its implementation.
6. Observer
	- Defines a subscription mechanism to notify multiple objects about any events that happen to the object they’re observing.
7. State
	- Allows objects to alter its behavior when its internal state changes. It appears as if the object changed its class.
8. Strategy
	- Defines a family of algorithms, put each of them into a separate class, and make their objects interchangeable.
9. Template Method
	- Defines the skeleton of an algorithm in the superclass but lets subclasses override specific steps of the algorithm without changing its structure.
10. Visitor
	- Separate algorithms from the objects on which they operate.