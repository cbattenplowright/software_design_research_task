# Software Design Research Task

### 1. What do we mean by **coupling** and **cohesion** when discussing structured design?

Coupling is the relationship between different elements of the program and how they interact with each other. Loose coupling is where elements have the minimum amount of dependence on other modules, tight coupling is the opposite. When designing software it is better to try and maintain loose coupling as it means each module is less dependent on other parts of the system making it easier to maintain and scale. 

Cohesion is the grouping of similarly functioning elements together. High cohesion is where a method/function should have a single, well-defined purpose. Software should try to maintain high cohesion to maintain readability and understanding of what that piece of the system should do.

### 2. What is the difference between **top-down** and **bottom-up** design? Which best describes a function oriented design?

A top-down design approach takes the software system as a whole and breaks it into sub-systems which are further broken down into their sub-systems giving a clear understanding of the overall system.

A bottom-up design begins with the most basic specific elements of the system and builds up to larger and larger parts of the program. This gives the benefit of focussing on the details of the individual components. 

With the design process of function oriented design, a top-down approach would be best as the design process focusses on the flow of data and the input and begins with a high level overview of the system before breaking it down logically into its sub-systems.

### 3. In which design methodology would a **class diagram** be most useful?

Class diagrams are most useful with object oriented design. With OOD using a bottom-up approach and classes being fundamental to how they work, class diagrams are helpful to map out the properties and behaviours of classes and how each class is related to other classes.

### 4. What are the **four pillars of object oriented programming**? Give a single-sentence description of each.

The four pillars are:

Abstraction - Abstraction is the process of only showing the essential features of an object and hiding the rest of the details away. 

Encapsulation - Encapsulation is the action of enclosing information and hiding the implementation of an object from the rest of the system and only making parts of the code accessible if needed.

Inheritance - Inheritance lets an object acquire the properties and behaviours of another object.

Polymorphism - Polymorphism is the ability of an object to take on different data types

### 5. What is the **strategy pattern**? How would its implementation differ between a functional and object oriented system?

The strategy pattern is a bevioural design pattern that allows you to dynamically change the behaviour of an object by encapsulating it into different strategies. By following this pattern it allows an object to change its behaviour at runtime without changing the code of the object itself.

Implementation of this pattern in a functional oriented system would be achieved by using functions. Each strategy is implemented as a function, and the component that needs to change its behaviour delegates the responsibilty of performing the behaviour to the appropriate function. 

In an object oriented system it would be implemented through the use of classes. There would be an abstract class which defines the behaviour all strategies must implement. Each strategy would then implement the abstract class and provide different implementations of the specified method behaviour that exists wihtin the interface. There would then be a further class which would be the object that delegates the responsibility of performing the behaviour to one of the strategies.

### 6. Imagine you are creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.

I would pick an object oriented design to create the online payment system. Reasons for this picking this design choice include reusability, modularity, readability and maintainability. 

Using encapsulation we can encapsulate data and behaviour together making the code secure. An example of encapsulation would be to contain sensitive data, like card details in objects.

Combining this with abstraction enhances the readability and maintainability of ths system. An example use would be abstracting the payment system. 

Using polymorphism can allow objects to behave in different ways. For example allowing the user to pay in multiple ways by using an interface of paymentMethod() and having it implemented in the different payment classes.