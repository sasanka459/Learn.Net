# INHERITANCE

* Inheritance is when a class child class gets the fields and methods of another class parent class.
* Inheritance is a way to form new classes using classes that have already been defined.
* Inheritance is a mechanism in which one class acquires the property of another class.
* Inheritance provides code reusability.

### Types of Inheritance
* **Single Inheritance**: A class inherits from one parent class.
* **Multilevel Inheritance**: A class inherits from another class, which in turn inherits from another class.
* **Hierarchical Inheritance**: Multiple classes inherit from a single parent class.
* **Hybrid Inheritance**: A combination of two or more types of inheritance.
* **Multiple Inheritance**: A class inherits from multiple parent classes.(Can be done using interfaces only.)


## EXAMPLES
 * **Single Inheritance**
 ```C#
 class Animal()
 {
 public void Legs()
 {
 Console.WriteLine("Animal has 4 legs"); 
 }
 }
 class Lion : Animal
 {
 public void Eat()
 {
 Console.WriteLine(" Lion eats meat");
 }
 }

 class Program 
 {
    static void Main() 
     {
        Lion l = new Lion();
        l.Legs(); 
        l.Eat();
      }
 }

 OUTPUT:    Animal has 4 legs
            Lion eats meat
```


* **Multilevel Inheritance**

 ```C#
 
 class Animal()
 {
 public void Legs()
 {
 Console.WriteLine(""); 
 }
 }
 
 class Lion : Animal
 {
 public void Eat()
 {
 Console.WriteLine("");
 }
 }
 
 class Tiger : Lion
 {
 public void Run()
 {
 Console.WriteLine("");
 }
 }
 class Program 
 {
    static void Main() 
     {
        Tiger t = new Tiger();
        t.Legs(); 
        t.Eat();
        t.Run();
      }
 }
 
 
 OUTPUT:    Animal has 4 legs
            Lion eats meat
            Tiger runs fast
```


* **Hierarchical Inheritance**

 ```C#
 class Animal()
 {
 public void Legs()
 {
 Console.WriteLine("Animal has 4 legs"); 
 }
 }
 
 class Lion : Animal
 {
 public void Eat()
 {
 Console.WriteLine(" Lion eats meat");
 }
 }
 
 class Tiger : Animal
 {
 public void Run()
 {
 Console.WriteLine(" Tiger runs fast");
 }
 }
 
 class Program 
 {
    static void Main() 
     {
        Lion l = new Lion();
        l.Legs(); 
        l.Eat();
        
        Tiger t = new Tiger();
        t.Legs();
        t.Run();
      }
 }
 
 OUTPUT:    Animal has 4 legs
            Lion eats meat
            Animal has 4 legs
            Tiger runs fast
```
 