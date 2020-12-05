Disclaimer: I have prepared these notes for reference of my own propose. Some of the contents are my own and some are re-quoted from textbook : "Data Structures: 
            Abstraction and Design Using Java, by Koffman and Wolfgang, John Wiley and Sons, 3rd edition, 2016 " and from my professor Dr. Jose Cordova.
            I in no way claim the ownership of the note or hold laibility of mistakes.These may be missing some important or basic concepts. I jolted down
            whatever felt I felt like to look back. Feel free to go through my notes or fork it to add your own notes or correct the mistakes. 

Inheritance
------------

    The extension of existing class is called inheritance.
    Inheritance creates a is-a relationship which means that child class is more specific version of parent class.

    If a class(child) inherits the class(parent class) i.e. child class has all the data fields and methods of the super class (must)
    but also a child class can have some more data field and methods than parent class.

    A subclass(child) can inherit the superclass(parent) by using the keyword 'extends' in the method declaration.

        Suppose a Bird class wants to inherit the Animal class it can do so by declaring it in class declaration.
            public class Bird extends Animal {}

    Note: if a data fields are created in super class using private keywords, child class cannot directly access it. So during the constructor
          creation of the subclass it has to use super() method invoking the constructor of the super class. If any argument constructor are in
          super class, pass the argument likewise in super() method. It has to be the first keyword used in constructor creation of subclass.

    Note: If no constructors are defined for a class, the no parameter constructor for that class is provided by default. However, if any constructors 
          are defined, you must explicitly define a no-parameter constructor.

    Note: variables with 'protected' keyword are accessible by any subclass or any class in a same package.


    Is-a Vs Has-a relationship
    --------------------------

    In an is-a or inheritance relationship, one class is a subclass of the other class. In a has-a or aggregation relationship, one class has
    the other class as an attribute.

    Methods Overriding
    ------------------

    Since inheriting the superclass will extract all its method to subclass which may seem trivial for subclass. We can modify it for subclass by
    having same method name, return type, declaration and parameters. We can write @override to make sure that we have successfully overriden the 
    parent class method. 

    Method Overloading
    ------------------

    Same method name but using the differenet number of parameter than the orginal method. It helps us to modify the existing method to work on only
    required arguments.
    
    Note: failing to override method successfully can sometimes result in method overload. so strictly annotate @override for better programming.



Polymorphism
------------

polymorphism is the standout feature of OOP.


    


