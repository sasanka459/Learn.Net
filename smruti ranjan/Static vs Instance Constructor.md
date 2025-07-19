# Instance vs Static constructor.

<details><summary> Instance Cosructor </summary>

* An instance constructor  is a special method in a class that  automatically runs when you create an object using new.
* Initializes the data of that specific object .
* Does NOT have a return type.
* We use instance constructor because it runs every time we use "new" keyword and it creates a new object.
* Each object can have different data each time its initialized.


``` C#
class new
{
    public string name;
    public int age;

    public new()
    {
        name = "tanisha" 
        age = 51;
    }
}

class Program
{
    static void Main()
    {
        Person p1 = new Person();
        Console.WriteLine(p1.name); 
        Console.WriteLine(p1.age);  
    }
}
OUTPUT:
        tanisha
        51

``` 
</details>

<details><summary> Static Constructor   </summary>

* A special constructor that initializes static data or performs actions that need to be done only once.
*  It’s automatically called by the runtime, before the first use of the class or any static members.
 * We cant call it manually.
 * no access modifiers can be used.
 * no parameters can be passed to it.
 
 ``` C#
 using System;

public class Sample
{
    public static int staticValue;

    // Static constructor
    static Sample()
    {
        Console.WriteLine("Static constructor called.");
       Value = 42; // Initialize static field
    }

    // Regular constructor
    public Sample()
    {
        Console.WriteLine("Instance constructor called.");
    }
}

class Program
{
    static void Main()
    {
       
        Console.WriteLine(Sample.staticValue);

        Sample obj1 = new Sample();
    }
}

Output  :
Static constructor called.
42
Instance constructor called.
```



</details>