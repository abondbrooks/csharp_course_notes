# **C# Notes**

C# is an object oriented programming language.

What is Object oriented programming?
- It is one of the most powerful methodologies in software development.
- It is used to create computer programs.
- It can speed up the program development process, imporove maintenance, and reusability.

- An **object** is the main concept or core concept involved in object orientation.
- An **object** is the representation of real world entities.
    * eg: a person, a pen, a bird, a chair
- It contains classes, objects and methods.

 ##
 **Characteristics of an object**

*The context of programming or object-oriented design refer to the fundamental aspects that define an object's nature and behavior within a program. Let's explain each characteristic simply:*


- **State**
    - The **state** of an object represents the current condition or data that the object holds at a particular moment.

    - These properties can be anything that describes the object, such as size, color, position, name, etc. For example, if we have an object representing a car, its state may include properties like "speed," "fuel level," "color," "number of doors," and so on.
- **Behavior**
    - The **behavior** of an object describes the actions or operations it can perform. In other words, it defines what the object can do or how it can interact with other objects in the program. 
    
    - These behaviors are typically represented by methods or functions that manipulate the object's state or perform certain tasks. For instance, continuing with the car example, behaviors of a car object may include "accelerate," "brake," "change gears," "honk horn," etc.

- **Identity**
    - The **identity** of an object is a unique characteristic that distinguishes it from other objects. It is a way to identify and reference a specific object within the program. The identity is usually assigned by the system and remains constant throughout the object's lifetime. 
    - In most programming languages, this identity is represented by a memory address or a unique identifier that ensures each object has its own separate existence. 
    - For instance, even if two cars have the same state (e.g., same color and speed), they would have different identities because they are different objects.

```csharp
using System;

class Car
{
    // State: Properties representing the attributes of the Car object
    public string Color { get; set; }
    public string Brand { get; set; }
    public int Speed { get; private set; }

    // Constructor to initialize the state of the Car object
    public Car(string color, string brand)
    {
        Color = color;
        Brand = brand;
        Speed = 0;
    }

    // Behavior: Methods that represent actions the Car object can perform
    public void Accelerate(int increment)
    {
        Speed += increment;
    }

    public void Brake(int decrement)
    {
        Speed -= decrement;
    }
}

class Program
{
    static void Main()
    {
        // Creating objects (instances) of the Car class

        // State: car1 object with color "red" and brand "Toyota"
        Car car1 = new Car("red", "Toyota");

        // State: car2 object with color "blue" and brand "Honda"
        Car car2 = new Car("blue", "Honda");

        // Accessing and modifying the state of the objects

        // Output the initial state of car1 and car2
        Console.WriteLine($"Car 1 - Color: {car1.Color}, Brand: {car1.Brand}, Speed: {car1.Speed}");
        Console.WriteLine($"Car 2 - Color: {car2.Color}, Brand: {car2.Brand}, Speed: {car2.Speed}");

        // Performing behaviors on the objects

        // Behavior: Accelerating car1 by 30 units
        car1.Accelerate(30);

        // Behavior: Accelerating car2 by 20 units
        car2.Accelerate(20);

        // Behavior: Braking car1 by 10 units
        car1.Brake(10);

        // Accessing the state after performing behaviors

        // Output the updated state of car1 and car2
        Console.WriteLine($"Car 1 - Color: {car1.Color}, Brand: {car1.Brand}, Speed: {car1.Speed}");
        Console.WriteLine($"Car 2 - Color: {car2.Color}, Brand: {car2.Brand}, Speed: {car2.Speed}");

        // Checking identity

        // Identity: Getting the unique identifier of car1 object
        Console.WriteLine("Identity of car1: " + car1.GetHashCode());

        // Identity: Getting the unique identifier of car2 object
        Console.WriteLine("Identity of car2: " + car2.GetHashCode());
    }
}
```

 **<center>Summary</center>**
  
    
*These characteristics together (state, behavior, and identity) form the basis of object-oriented programming and help in creating and manipulating objects to model real-world entities or abstract concepts in software development.*

**Four Pillars of Object-Oriented Programming**

*The **four pillars of object-oriented programming (OOP)** are:*

- **Abstraction:**
Abstraction is the process of simplifying complex real-world entities into essential and relevant characteristics, ignoring the irrelevant details. In OOP, abstraction is achieved through abstract classes and interfaces. Abstract classes define common attributes and behaviors for subclasses, while interfaces define a set of methods that classes must implement. Abstraction allows programmers to model real-world objects and systems effectively.

- **Polymorphism:**
Polymorphism allows objects of different classes to be treated as objects of a common superclass. It enables a single interface to represent multiple forms or types of objects, providing flexibility and reusability in code. Polymorphism can be achieved through method overriding (runtime polymorphism) and method overloading (compile-time polymorphism). This feature allows different objects to respond differently to the same method call based on their specific implementation.

- **Inheritance:**
Inheritance is the process by which one class (subclass or derived class) inherits the attributes and behaviors of another class (superclass or base class). It establishes a hierarchical relationship between classes, promoting code reusability and the creation of specialized classes. Subclasses can extend the functionality of the superclass and override its methods to provide their implementations. Inheritance forms an "is-a" relationship, where a subclass is a specialized version of its superclass.

- **Encapsulation:**
Encapsulation is the concept of bundling data (attributes) and the methods (behaviors) that operate on the data within a single unit called a class. It hides the internal implementation details of an object from the outside world, and access to the object's data is restricted to specific methods defined within the class. Encapsulation promotes data protection, code modularity, and ensures that the object's state is maintained consistently through its methods.

**<center>Summary</center>**

*These four pillars are fundamental principles of OOP and play a crucial role in designing and developing software with qualities such as flexibility, maintainability, and scalability. By utilizing these principles, programmers can build more organized, efficient, and understandable code, leading to better software solutions.*


**Software Development Life Cycle (SDLC)**

*The **Software Development Life Cycle (SDLC)** is a framework that provides a structured approach to the development of software. It consists of a series of phases that guide the software development process from the initial concept to the final deployment and maintenance.* 

*The stages in **SDLC** are as follows:*

- **Requirement Gathering:** Gathering and understanding the software requirements from stakeholders, users, and clients.
- **Analysis:** Analyzing the requirements to define the project scope, constraints, and objectives.
- **Design:** Creating a detailed design plan that outlines how the software will be structured and developed.
- **Implementation:** Writing the actual code and building the software based on the design.
- **Testing:** Conducting various testing activities to ensure the software functions correctly and meets the requirements.
- **Deployment:** Releasing the software to end-users or clients.
- **Maintenance:** Providing ongoing support, bug fixes, and updates to the software throughout its lifecycle.

 **<center>Summary</center>**

*These stages are essential in ensuring the successful development of software that meets user needs, is of high quality, and can be easily maintained and updated throughout its lifecycle. The **SDLC** provides a systematic approach, and each stage contributes to the overall success of the software project.*

**Compiler**
- It is a software program which converts the code to machine code.

**.Net Framework**
- It is a technology that supports building and running applications.

- It is the foundation of which we design, develop and deploy applications.

- .Net framework consists of CLR (Common Language Runtime), CLS (Common Language Specifications), CTS (Common Type System) and the JIT (Just-in-time) Compiler.

**CLR (Common Language Runtime)**

- It is one of the most essential components in the .net framework.

- It is the enviorment where all the programs using .net technologies are executed.

 **<center>Summary</center>**

***Compiler:** A software program that converts human-readable code into machine code for a computer to understand and execute.*

***.NET Framework:** A technology platform that facilitates building and running applications. It comprises essential components like CLR, CLS, CTS, and the JIT Compiler.*

***CLR (Common Language Runtime):** An integral part of the .NET Framework where .NET applications are executed. It provides the environment for running programs using .NET technologies.*

 