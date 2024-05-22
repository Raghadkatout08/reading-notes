# Design Patterns | Strategy Pattern | SOLID Principles | Enum in Python

## Python Design Patterns

Design patterns are crucial in software engineering, offering repeatable solutions to common problems in software design. They encapsulate best practices by experienced object-oriented developers, serving as templates rather than direct code solutions.

### Classification of Design Patterns
* Creational Design Patterns 
    - Focus on object instantiation.
    - Categories: Class Creational Patterns (use inheritance) and Object Creational Patterns (use delegation).
    - Types:
        - Factory Method
        - Abstract Factory Method
        - Builder Method
        - Prototype Method
        - Singleton Method

* Structural Design Patterns
    - Organize classes and objects to form flexible, efficient structures.
    - Use inheritance for interface composition and relationship simplification.
    - Types:
        - Adapter Method
        - Bridge Method
        - Composite Method
        - Decorator Method
        - Facade Method
        - Proxy Method
        - Flyweight Method


* Behavioral Design Patterns
    - Identify common communication patterns between objects.
    - Concerned with algorithms and responsibility assignments.
    - Types:
        - Chain of Responsibility Method
        - Command Method
        - Iterator Method
        - Mediator Method
        - Memento Method
        - Observer Method
        - State Method
        - Strategy Method
        - Template Method
        - Visitor Method


### Advantages of Using Design Patterns


* `Reusability`: Enhance code reuse across multiple projects.
* `Transparency`: Improve code transparency for future developers.
* `Established Solution`: Provide well-proven, reliable solutions.
* `Efficient Communication`: Facilitate better communication among designers by referencing patterns.
* `Efficient Development`: Aid in creating highly cohesive, minimally coupled modules


## SOLID Principles in Python

The SOLID principles are a set of five design guidelines. Martin (Uncle Bob). They are intended to help developers create more maintainable, understandable, and flexible software.

* SOLID Principles:

    - Single Responsibility Principle (SRP):
        Definition: A class should have only one reason to change, meaning it should have only one job or responsibility.
        Example: In Python, a class responsible for managing user data should not handle user interface logic.

    - Open/Closed Principle (OCP):
        Definition: Software entities (classes, modules, functions, etc.) should be open for extension but closed for modification.
        Example: You should be able to add new methods to a class without altering existing ones, often achieved through inheritance or interfaces.

    - Liskov Substitution Principle (LSP):
        Definition: Subtypes must be substitutable for their base types without altering the correctness of the program.
        Example: If a base class Bird has a method fly(), any subclass like Sparrow or Eagle should implement fly() in such a way that it works seamlessly in place of Bird.


    - Interface Segregation Principle (ISP):
        Definition: Clients should not be forced to depend on interfaces they do not use. This principle encourages the creation of more specific interfaces rather than one general-purpose interface.
        Example: In Python, instead of having a large interface Animal with methods like fly(), swim(), walk(), create smaller, more specific interfaces like FlyingAnimal, SwimmingAnimal, and WalkingAnimal.

    - Dependency Inversion Principle (DIP):
        Definition: High-level modules should not depend on low-level modules but on abstractions. Additionally, abstractions should not depend on details, but details should depend on abstractions.
        Example: In Python, use dependency injection to pass dependencies to a class rather than instantiating them within the class. This way, the class relies on abstract interfaces rather than concrete implementations.

* Benefits of SOLID Principles:
    - Maintainability: Makes the codebase easier to maintain and extend over time.
    - Flexibility: Enhances the ability to change or add new functionality without breaking existing code.
    - Scalability: Facilitates building scalable applications by promoting decoupled and cohesive code.


## Enum in Python

Enumerations, or Enums, are a data type that consists of a set of named values called members. Enums help define variables that can hold a set of predefined constants, which enhances code readability and maintainability.

* Key Points:
    - Definition and Purpose: Enums are used to define a collection of related constants, providing clear and meaningful names for these values.
    - Creation: Enums are created using the Enum class from the enum module.
    - Accessing Members: Enum members can be accessed using their names or values.
    - Iteration: Enums can be iterated over to access each member.
    - Comparison: Enum members can be compared using identity and equality operations.
    - Auto-Assignment: The auto() function can be used to automatically assign values to enum members.
    - Methods: Enums can have methods to add functionality.
    - Benefits: Enums improve code readability, maintainability, and help reduce errors by limiting the set of possible values for a variable.
    - Enums are a useful feature in Python for managing sets of related constants in a clear and organized way.



## References

* [Design Patterns](https://www.geeksforgeeks.org/python-design-patterns/)

* [SOLID Principles](https://www.youtube.com/watch?v=pTB30aXS77U)

* [Enum in Python](https://www.geeksforgeeks.org/enum-in-python/)