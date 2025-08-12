# POLYMORPHISM
* Polymorphism is derived from the Greek words "poly" (meaning many) and "morph" (meaning forms).
* In pilymorphism,You can use the same method or object name to perform different tasks.
* It is a feature of OOP that allows one interface to be used for different data types.
* Polymorphism allows methods to do different things based on the object it is acting upon.
* Polymorphism is the ability of different classes to be treated as instances of the same class through a common interface.
* polymorphism is of two types.
	1. Compile-Time Polymorphism(Method Overoading)
	1. Run-time Polymorphism(Method Overriding)

## Compile-Time Polymorphism(Method Overoading)

* In this type of polymorphism, the method to be executed is determined at compile time (before the program runs).
* Method Overloading means creating multiple methods with the same name in the same class, but with:
1. Different number of parameters
2. different type of parameters
 * It allows us to call the same method name in different ways depending on the arguments we pass.

 ### EXAMPLE
 ```C#
 using System;

class Addition {
    
    public int Add(int a, int b) {
        return a + b;
    }

       public double Add(double a, double b) {
        return a + b;
    }

    public int Add(int a, int b, int c) {
        return a + b + c;
    }
}

class Program {
    static void Main() {
        Addition calc = new Addition();
        Console.WriteLine(calc.Add(5, 10));        
        Console.WriteLine(calc.Add(3.5, 4.5));     
        Console.WriteLine(calc.Add(1, 2, 3));      
    }
}
```
##  Run-time Polymorphism(Method Overriding)

* It is called run-time because the method call is resolved at runtime, depending on the object type (not reference type).
* It also known as Dynamic Polymorphism.
* We need a base class with a method marked with  virtual keyword .The virtual keyword is used to mark a method in a base class as being "overridable" by the child classe. 
* A derived class with a method marked as override. Which allows us to override the parent class marked with virtual keyword.


### EXAMPLE
```C#
using System;

class Animal  
{
    public virtual void Speak()  
    {
        Console.WriteLine("The animal makes a sound.");
    }
}

class Dog : Animal  
{
    public override void Speak() 
    {
        Console.WriteLine("The dog barks.");
    }
}

class Cat : Animal  
{
    public override void Speak()
    {
        Console.WriteLine("The cat meows.");
    }
}

class Program
{
    static void Main()
    {
        Animal myAnimal = new Animal();
        Animal myDog = new Dog();  
        Animal myCat = new Cat();  

        myAnimal.Speak(); 
        myDog.Speak();    
        myCat.Speak();
    }
}
Output:  The animal makes a sound.
                 The dog barks.
                 The cat meows.
```
