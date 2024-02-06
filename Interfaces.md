An interface is an [[Abstract Classes]] that is used to descend its methods and properties to descendant classes

https://docs.oracle.com/javase/tutorial/java/IandI/createinterface.html

In the Java programming language, an _interface_ is a reference type, similar to a class, that can contain _only_ constants, method signatures, default methods, static methods, and nested types. Method bodies exist only for default methods and static methods. Interfaces cannot be instantiated—they can only be _implemented_ by classes or _extended_ by other interfaces. Extension is discussed later in this lesson.

Defining an interface is similar to creating a new class:

```Java
public interface OperateCar {

   // constant declarations, if any

   // method signatures
   
   // An enum with values RIGHT, LEFT
   int turn(Direction direction,
            double radius,
            double startSpeed,
            double endSpeed);
   int changeLanes(Direction direction,
                   double startSpeed,
                   double endSpeed);
   int signalTurn(Direction direction,
                  boolean signalOn);
   int getRadarFront(double distanceToCar,
                     double speedOfCar);
   int getRadarRear(double distanceToCar,
                    double speedOfCar);
         ......
   // more method signatures
}
```