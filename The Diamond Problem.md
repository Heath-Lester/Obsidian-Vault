
https://en.wikipedia.org/wiki/Multiple_inheritance

This is a problem of indecisiveness that is created when two parent classes of the same ancestor/superclass have an different implementations of an inherited method from said grandparent/ancestor.


https://shahedbd.medium.com/why-oop-does-not-support-multiple-inheritance-c2f99824a104

Because of this, some languages flat out do not support multiple inheritance. Another implication of this is that the structural design pattern, the adaptor pattern, cannot be implemented in languages that do not support multiple inheritance.

In spite of this, languages generally provide ways to work around this issue. Java, for example, allows the implementation of multiple interfaces in a single class. Because interfaces are abstract, and do not enforce the implementation, the methods inherited from the interfaces do not need to decide which implementation to use.



