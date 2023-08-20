## Things I want to know more about
# class6


Q1. What is the difference between an Object and a Class in Java


<pre> 

Object: An object is a fundamental concept in object-oriented programming (OOP). It's a self-contained unit that combines both data (state) and the functions (behavior) that operate on that data. Objects are used to model real-world entities or concepts within a software system. Each object represents a specific instance of a class and can have its own unique state and behavior.

Class: A class is a blueprint or template that defines the structure and behavior of objects. It encapsulates the common attributes (state) and methods (behavior) that objects of that class will possess. A class provides a reusable and organized way to create objects with consistent properties and behaviors. Objects are instances of classes, meaning they are created based on the specifications provided by the class.

</pre>


Q2.Explain to a non-technical friend the concept of inheritance in Java.
<pre>

Imagine you have a family: a dad and a child. The dad has some traits, like his name and his ability to cook, and he can also do some things, like driving a car. Now, the child is part of the family and has similar traits because they inherit things from their dad.

class Dad {
    String name;

    void cook() {
        System.out.println(name + " is cooking dinner.");
    }

    void drive() {
        System.out.println(name + " is driving the car.");
    }
}





class Child extends Dad {

void play() { System.out.println(name + " is playing with toys."); } }





now the child inherited all thing from the dad



</pre>
Q3 .Static methods are also called what? Why?
<pre>
we can use the static keyword in Java.  to access class members without creating an instance of the class, we need to declare the class members static.

Static methods are also called class methods. It is because a static method belongs to the class rather than the object of a class.

And we can invoke static methods directly using the class name.
</pre>

Q4. How can you access a variable of a class without instantiating an object from that class?
<pre>

when you're inside the same class where the static variables are defined, you can access it directly without using the class name.


we can accessing the static variable from the other class using the class name. like :

class Test {
    // static variable
    static int age;
}
class Main {
    // access the static variable
    Test.age = 20;
}


</pre>

Q5. What is a Design Pattern? Describe one or two with analogies from your previous work experience.
<pre>
Patern: Design patterns are reusable solutions to common problems that arise during software design and development. Using design patterns can save time, improve code quality, and promote best practices in software design.

singleton Pattern: Imagine a unique key that opens a treasure chest. The Singleton pattern ensures that there's only one key in existence, allowing access to a shared resource. No matter how many people want to open the treasure chest, they all use the same key to access its contents.

AAA stands for "Arrange, Act, Assert pattern >>this pattern helps make your tests more readable and understandable by separating the different phases of a test case.
</pre>
Q6.What is a Singleton
<pre>
Singleton is a design pattern that ensures that a class can only have one object.

To create a singleton class:

Create a private constructor of the class
Create a private attribute of the class type
Create a public static method that allows us to create and access the object we created. 


</pre>
