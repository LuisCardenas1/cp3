# cp3

2/7/2022
Polymorphism

Class A has-an instance of class B
Aggregation (Has-A) is a one way to share data classes
Can only use public parts
Another way to share data is inheritance
There is a base class with classes that extend from it
New class word: extends
Defines the inheritance relationship
UML: Arrow with open head
Class A extends class B;
Inherits everything from class B AND allows us to add to it
New method/data visibility keyword: protected
This data item/method is visible both inside the class and to classes that extend this class
Also visible to other classes in the same package 
"#" in UML

Subclass can be called: Child class
Superclass can also be called: Parent class, Base class

Subclasses get direct access to all of the public and protected data methods from superclass
  May have to implement methods again if we need more specific behavior
 
The relationship represented by aggragation(with the diamond in UML) is "has-a"
The relationship represented by inheritance(with the open headed arrow) is a "is-a"

Inheritance is good in GUI components, and collections
Inheritance breaks encapsulation if we use the protected keyword
Aggregation/compositition do not break encapsulation

If everything is private:
  Inheritance doesn't provide the subclass itself with anything it can't get through composition
  However: the "user" of a class does get to see a consistent interface between the super and child classes
If everthing is protected:
  Classes can be closely coupled
    Changes in one are likely to cause changes in the other
    
2/9

Overriding Methods
  When a subclass implements a method that is identical to one in the superclass, it overrides the superclass method
    Superclass method must be public or protected
    Same name
    Same parameters
    Return values: new method must return a subclass of the original method's return type
    Static methods cannot be overridden
    
Use instanceof when downcasting
