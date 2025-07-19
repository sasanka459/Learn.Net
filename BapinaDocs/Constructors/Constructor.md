### Constructor

- It is a specal method of the class which is use to initialize the instance variable.
- Constructor of a class must have the same name as the class name because of the easy identification of the compilier.
- It can't be abstract class,within a class you can creat only one static constructor,a class can have any number of constructor,access modifier can use in constructor.
- Constructor have 5 types:-
 1-Default con:-A constructor with no parameters is called a Default constructor.
 2-Parameterized co:-A constructor having at least one parameter is called a parameterized constructor.
 3-Copy con:-A copy constructor is used to create a new object by copying the values from an existing object of the same class.
 4-Private con:-If a constructor is created with a private specifier is known as Private Constructor.
 5-Static con:-it is invoke one and only once when the class has been loaded into the application domain.it is also use to initialize the static variable.static constructor must be parameter less.
               Non-static constructors can be overloaded but not the static constructors. Overloading is done on the parameters criteria. So if you cannot pass the parameters to the Static constructors then we can't overload it.
                                                                                     
### Example of Constructor

```C#
public class car
{
    public string name;
    public car()
    {
        name="mustang";
    }
    public static void Main(string[] args)
    {
      car c=new car();
      Console.WriteLine(c.name);
    }
}

```

### Example of static con

``` c#
public class Message
{
    static Message()    /// Static con
    {
        Console.WriteLine("this is static Constructor");
    }
    public Message()   ///non static con or con
    {
        Console.WriteLine("this is non static Constructor");
    }
    public static void Main(string[] args)
    {
        Message obj1=new Message();
         Message obj2=new Message();
    }
}
```

### static constructor must be parameter less

``` C#
public class Message
{
    static int x;  /// static variable
    static Message(int k)   //Passing a Parameter ( when you run tha program it showing error because  a static constructor must be parameterless)
    {
        k=x;
        Console.WriteLine("this is static and k= "+k);
    }
    public Message()
    {
        Console.WriteLine("this is non static");
    }
    public static void Main(string[] args)
    {
        Message obj1=new Message();
         Message obj2=new Message();
    }
}
```

### instance constructor
```C#
public class car
{
    //instance field
    public string model;
    public string color;
    public int year;
        //Instance Constructor  (with parameters)
    public car(string modelname,string modelcolor,int modelyear)
    {
        model=modelname;
        color=modelcolor;
        year=modelyear;
    }
    public static void Main(string[] args)
    {
        car c=new car("siaz","red",2022);
        Console.WriteLine(c.model+" "+c.color+" "+c.year);
    }
}
```








