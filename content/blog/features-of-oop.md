---
title: "Features of Object Oriented Programming"
date: 2021-03-21T13:06:26+06:00
featureImage: images/allpost/oop-tn.png
postImage: images/single-blog/feature-image.jpg
---

### What is Object Oriented Programming?
Object-Oriented Programming (or OOP) is the most widely used programming paradigms used in the Computing industry. Many programming languages offer an Object-Oriented approach such as C#, JavaScript, and PHP. 

Object-Oriented Programming relies on a class and object based system, in which code is recycled and reused for use at multiple points throughout the program.

### Advantages of Object Oriented Programming
+ Allows for faster program development as most Object-Oriented programming languages are equipped with large libraries of recyclable code during previous projects which allows it to be used for future projects; thus, reducing the cost of development and being able to allocate additional resources to processes such as Object-Oriented design and analysis. 
+ Improved productivity. Object-Oriented programming as a whole is modular as it is scalable, meaning that objects can be ‘extended’ to withhold new attributes and other features. This is useful in games as if the developers want to add a new feature to the game, it’s easier just to create a new class and mould the original program around this new class. You’re able to just “bolt on” this class which as a result, makes the program scalable. As a result of the three factors - modularity, scalability, and reusability, Object-Oriented Programming provides the developer with robust programming productivity as opposed to a procedural-based technique. 
+ Finally, it allows the programmer to maintain and develop high-quality software. As a result of the reduced cost and time, more resources can be allocated towards verifying and testing the software; thus resulting in high standard software.

### Disadvantages of Object Oriented Programming
+ Object-Oriented programs are quite large in size as they have considerably more lines of code and files than procedural programs. Larger programs cause it to ultimately become increasingly slower as they typically require more instructions to be executed. 
+ It has a very steep learning curve as the thought process required to make Object-Oriented is much more complex as opposed to Procedural or Event-Driven Programming. Object-Oriented relies on the programmer to make applications based on interacting with Objects. In addition to this, some key components of OOP such as Abstraction and Encapsulation can be quite difficult to understand for someone new to programming. 
+ Finally, it’s not a viable technique for all types of programs. There are some programs that would work much more efficiently in a procedural-based environment as opposed to an object-based environment.

### Encapsulation
Encapsulation is the first of the four principles of Object-Oriented Programming. It focuses on combining data into a bundle and methods that work within a single unit, for example, a class in Java. It is also used to hide internal representation or state of an object externally. In any Object-Oriented Programming language, these are known as ‘get’ and ‘set’ methods. 

+ The ‘get’ method is used to access an attribute for the programmer to later modify.
+ The ‘set’ method allows you to edit the attribute and change it depending on your preferences. 

You can implement ‘information-hiding’ mechanisms by changing your class attributes to become inaccessible from the outside; alongside giving ‘get’ and ‘set’ methods for attributes which should either be readable, or updated by any other class. 

C# supports 6 different ‘Access Modifiers’ (public, private, protected, internal, protected-internal, private-protected) which can define whether or not the programmer can edit attributes from x file. However here, I’m only going to focus on ‘public’ and ‘private’ modifiers. 

+ The public modifier allows the developer to access a certain type or member by other code from within the same program or one at which references it. 
+ The private modifier only allows the developer to access the type or member within the same class. 

Encapsulation withholds many advantages, being one of the core principles you must learn if you’re getting into the Object-Oriented paradigm. 

+ It secures data stored within the program, stopping unauthorized users from accessing sensitive information. 
+ Encapsulation heavily reduces the maintenance needed for the application. Reducing the maintenance needed for the application will further save time and money for the developer(s). 
+ It makes the applications source code easier to understand by other developers that might work within your team. 
+ It simply reduces human error, allowing the programmer to work more efficiently on the delegated activities. 

Encapsulation makes your code modular by mapping encapsulated objects into physical modules. Using the recycled code provided by the use of modularity, programmers can use parts of this reused code to form that physical module. Modularity refers to constructing modules and combining them to bundle together a system; essentially allowing you to reuse and recycle code instead of duplicating it. In addition to this, it also makes it easier for debugging and bug fixing as bugs can be traced to the specific module; thus focusing the scope of in-depth error searching. 

### Inheritance
Inheritance allows classes to inherit features of other classes which maintain similarities. This means that there are two types of classes which are needed; a ‘child’ class which derives from a ‘parent’ class; thus forming a hierarchy. This way, each class only adds what's needed by reusing common logic within the parent class. 

For example, a ‘parent’ class could be an Enemy class with a ‘health’ attribute. Each ‘child’ class could be an individual enemy identifier e.g. Vampire. The health attribute will vary depending on what enemy it is, in this instance, "Vampire" has 50 health. With that being said, inheritance has many advantages. 

+ Inheritance promotes reusability; when a class inherits or derives another class which allows it to access all functionality of the parent class. Using parent classes diminish the need for code duplication which can consequently reduce the building time of an application. 
+ Helps to reduce code redundancies, allowing the program to support code extensibility. 
+ Inheritance makes the ‘child’ classes follow a specific path; for example, a dog may be able to walk, but it seems redundant to duplicate the code needed to make the dog walk. However, putting this in a ‘parent’ class essentially constructs a blueprint for the child class to follow. 

Inheritance also has some disadvantages.

+ Incorrect usage of inheritance can cause distorted solutions. This can lead to another disadvantage that it can make the program slower than needed as an overuse of attributes, leading to memory wastage as well as becoming inconvenient in certain cases. 
+ It increases coupling between parent and child classes. A change in the parent class will affect all child classes which could cause bugs for multiple classes as opposed to a singular class.

```
using System;

class Car 
{
    public string brand = "Ford";
    public void honk() 
    {
        Console.WriteLine("Honk, honk!");
    }
}

class Motorbike : Car 
{
    public string modelName = "BMW";
}

class Program 
{
    static void Main(string[] args) 
    {
        Motorbike myMotorbike = new Motorbike();
        myMotorbike.honk();
        Console.WriteLine(myMotorbike.brand + " " + myMotorbike.modelName);
    }
}
```

### Polymorphism
Polymorphism is another one of the core principles of the Object-Oriented paradigm. It can be used in a variety of contexts at which something will occur in multiple circumstances or forms. It outlines a theory to which objects of different types can be accessed through a common interface. There are two different types of Polymorphism which I’m going to discuss; ‘Static’ and ‘Dynamic’. 

+ Static Polymorphism refers to the implementation of various methods within the same class that share a common identity, but represent an alternate set of parameters; this is something called ‘method overloading’ that represents the ‘static’ form of Polymorphism. As a result of the different sets of parameters, each method produces a different signature, allowing the compiler to recognise what method needs to be called. 
+ Dynamic Polymorphism doesn’t enable the compiler to choose the chosen method. Surrounding the hierarchy of inheritance, a child class is able to override a method of it’s parent class in order to modify or completely renovate the behaviour of the selected method. This is especially important with Object-Oriented programming as it allows the programmer to be able to reuse their code for purpose at a later date. When creating something like a game, the developer could use a parent class to inherit the health of an enemy to a vampire, which in this instance would be your child class. This can ultimately be achieved by using virtual methods. 

Polymorphism encompasses many advantages.

+ Extensibility or ‘Scalability’ is a principle which provides opportunity for future growth upon an existing product.
+ Polymorphism allows us as programmers to write clear, clean and well-structured code that knows little about the types it is dealing with. 
+ Separation of concerns (known in the Computer Science industry as SoC) which is a design principle for splitting up a program into separate sections such that each area of the program appeals to a separate topic.

On the other hand to any advantages of Polymorphism, there are also some disadvantages. 

+ During runtime Polymorphism can cause performance issues as the device needs to determine the method or variable to call; thus depriving the performance and decisions taken during runtime. 
+ Polymorphism decreases the readability of the program's source code. To identify the execution time of the program, you need to pinpoint the runtime behaviour.

```
using System;

class Car 
{
    public void carSound() 
    {
        Console.WriteLine("Broom, Broom!");
    }
}

class Skoda : Car 
{
    public void carSound() 
    {
        Console.WriteLine("Vroom, Vroom!");
    }
}

class Mercades : Car 
{
    public void carSound() 
    {
        Console.WriteLine("Neeeowmmm!");
    }
}
```

### Abstraction

Abstraction is the last of the four main principles of Object-Oriented Programming. Abstraction essentially refers to user interaction with specific attributes and methods of an object; using simplified versions of upper-level tools in order to access a complex object. In short, Abstraction uses simple classes to represent complexity; whilst extending upon another one of the main principles of Object-Oriented Programming; Encapsulation.

For example, you don’t need to know how the engine works to drive a Car as the driver will only use a small range of devices: like the breaks, steering wheel, and the gear stick. However, to make the car work, there are a lot of different mechanisms and parts that have to work in the engine - though my point still stands, these types of details don’t need to be disclosed to the driver. On the more technical side, abstraction can be achieved using specific abstract classes or similarly, interfaces. 

The C# programming language contains a “abstract” keyword which can be used for use to create specific abstract classes and methods. An abstract class is a restricted class that is unable to be used to create objects; but it can be accessed by inheriting it from another class. They can also contain both abstract and normal methods. Additionally, there are also abstract methods available. These are only able to be used within an abstract class with a body derived from another derived class. 

There are many different advantages surrounding Abstraction.

+ The interface provides security and protects the implementer from incorrect use of a data structure by the client. The interface then proceeds to create an abstraction barrier that safeguards the implementation. 
+ When the developer adds something else or updates the code, it rarely hinders the process of Abstraction allowing for easier software maintenance. 

On the contrary, Abstraction also has drawbacks. 

+ Though the code size doesn’t normally affect most modern systems, it can be a crippling problem on smaller devices. Extra code needed to completely include Abstraction within the program ultimately includes additional code, leading to overlarge runtime executables which results in the device much more pricey.

```
using System;

abstract class Car 
{
    public abstract void carSound();
    public void brake() 
    {
        Console.WriteLine("Skrrrrr!");
    }
}
```

### Properties
Properties are characteristics or ‘attributes’ of an object. For example, an Object could be a car with attributes such as colour, weight, and petrol-type. You could explain a property like a variable that is essentially ‘linked’ or attached to an object. For example, A Jaguar may be White weighing ~2300kg and a petrol-based car and another Jaguar could be Black, weighing the same with a diesel-based engine. 

Properties support different access modifiers which can let properties access a classe. The two modifiers which are primarily used are the public and private modifiers. The public modifier allows the developer to access a certain type or member by other code from within the same program or one at which references it. However, the private modifier only allows the developer to access the type or member within the same class. You can access the properties of an object by using something called ‘dot notation’.

### Methods
Methods represent the behaviour or the actions of an object. For example, a car will have methods of brakes, steering, and shifting gears. Methods carry out actions, return information, or update an object's data. This is the main way programmers reuse their code. One of the most vital capabilities of methods within Object-Oriented Programming is of which it provides method overriding. It allows multiple classes to use the same method but ‘override’ some of the behaviours of the methods within that specific class. 

Methods also provide the interface that the other classes use to access and edit the properties of an object; as stated in a previous section, this is also known as Encapsulation. Encapsulation and method overriding are two of the main differences between that of methods and procedural calls. You can denote a protected variable by adding an underscore to the front of the declaration - for example, _steering. 

To finalise this section on methods, I am going to discuss two alternating types of methods; constructors and destructors. 

+ A constructor is a special method used with a class for instantiating and initializing an object within that class. 
+ Destructors in memory-managed programming languages such as C#, are known as ‘Finalizers’. A destructor can be implemented to perform ‘cleanup chores’ throughout the program to allow for more memory allocation. The difference between a normal destructor and finalizer is only that the sequence that they are called is slightly different.

### Classes
Classes are normally used to create blueprints for broader categories such as Car or Animal that would have something in common. For example, a Car class will have similar attributes to all objects within the class; like driving and breaking. An Object is an instance of a class which contains methods and properties to construct particular types of useful data. It can also contain a data structure, variable, or even a function. As you can see, although they are used together, there are differences between the two. A class system enables the program to define a derived class in terms of a ‘parent’ class by using features such as inheritance, overriding and augmenting.

### UML (Unified Modelling Language)
UML is short for Unified Modelling Language. It consists of a set of diagrams and visual representations developed to assist software and system developers for visualizing, constructing, and documenting sections of software systems. However, it can also be used for business models and various non-software related systems. UML is a vital part of developing Object-Oriented applications; mainly graphical notations to express the design of software-based  projects. 

It is used by project teams to communicate, explore potential designs, and confirm designs of software. Behaviour diagrams represent dynamic behaviour of objects within a system. Though there are seven different types of these diagrams, I am only going to discuss the Class and the use-case Diagram in this question. 

The class diagram models the static structure of a system, whilst representing the relationship between classes, objects, attributes, and operations. The class diagram takes the static structure of the application or program, and requires the programmer to translate it into code. Within the diagram, three types of principles regarding relationships between the nodes are important: association, inheritance, and aggregation. 

The use-case diagram expresses a system's functional requirements using a method known as ‘cases’. It allows you to envision what you need from a system to how the  system can meet those needs. The easiest way to think of a use-case diagram is like a menu; the individual products along with the cost of each dish on the menu. This way, you get a feel to what type of cuisine the restaurant serves such as Italian, Chinese, and American; thus modelling the restaurant's behaviour.