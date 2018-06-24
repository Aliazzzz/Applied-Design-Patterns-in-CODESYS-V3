# Applied-Design-Patterns-in-CODESYS-V3

I picked up these design-patterns from various sources all around the internet and decided to share them.
Ideal for selfstudy purpose. Kudo's go out to the original posters!

Design Patterns can be divided by three types;
Creational patterns are ones that create objects for you, rather than having you instantiate objects directly. This gives your program more flexibility in deciding which objects need to be created for a given case.

    Abstract factory pattern groups object factories that have a common theme.
    Builder pattern constructs complex objects by separating construction and representation.
    Factory method pattern creates objects without specifying the exact class to create.
    Prototype pattern creates objects by cloning an existing object.
    Singleton pattern restricts object creation for a class to only one instance.

Structural
These concern class and object composition. They use inheritance to compose interfaces and define ways to compose objects to obtain new functionality.

    Adapter allows classes with incompatible interfaces to work together by wrapping its own interface around that of an already existing class.
    Bridge decouples an abstraction from its implementation so that the two can vary independently.
    Composite composes zero-or-more similar objects so that they can be manipulated as one object.
    Decorator dynamically adds/overrides behaviour in an existing method of an object.
    Facade provides a simplified interface to a large body of code.
    Flyweight reduces the cost of creating and manipulating a large number of similar objects.
    Proxy provides a placeholder for another object to control access, reduce cost, and reduce complexity.

Behavioral
Most of these design patterns are specifically concerned with communication between objects.

    Chain of responsibility delegates commands to a chain of processing objects.
    Command creates objects which encapsulate actions and parameters.
    Interpreter implements a specialized language.
    Iterator accesses the elements of an object sequentially without exposing its underlying representation.
    Mediator allows loose coupling between classes by being the only class that has detailed knowledge of their methods.
    Memento provides the ability to restore an object to its previous state (undo).
    Observer is a publish/subscribe pattern which allows a number of observer objects to see an event.
    State allows an object to alter its behavior when its internal state changes.
    Strategy allows one of a family of algorithms to be selected on-the-fly at runtime.
    Template method defines the skeleton of an algorithm as an abstract class, allowing its subclasses to provide concrete behavior.
    Visitor separates an algorithm from an object structure by moving the hierarchy of methods into one object.



# Remember kids!

Allthough design patterns can ease your life significantly, the best solution is always the simplest solution no matter what fancy pattern you throw at it!

Significant criticism has been directed at the concept of software design patterns generally, and at Design Patterns specifically.

A primary criticism of Design Patterns is that its patterns are simply workarounds for missing features, replacing elegant abstract features with lengthy concrete patterns, essentially becoming a "human compiler" or "generating by hand the expansions of some macro". 
