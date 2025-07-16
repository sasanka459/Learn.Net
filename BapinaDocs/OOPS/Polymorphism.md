### Polymorphism

- Polymorphism means "many forms", means the same method can perform different operations in different scenarios.
- There are two types

 1-Static / Compile Time Polymorphism
- It is also known as early binding.if the binding process carried out at the time of compilation is called early binding.
-     Overloading-we can create multiple methods of the same name in the same class  and parameters are diffrent and all methods works in diffrent way.
  
- ### example of overloading
``` C#
    public class sum
     {
    public int add(int a,int b)
    {
        return a+b;
    }
    public int  add(int a,int b,int c)
    {
        return a+b+c;
    }
      }
      public class HelloWorld
    {
    public static void Main(string[] args)
    {
        sum s=new sum();
        int x=s.add(10,20);
        int y=s.add(10,20,30);
        Console.WriteLine("sum of 2 int is : "+x);
        Console.WriteLine("sum of 3 int is : "+y);  
      }
    }
```


 2-Dynamic / Runtime Polymorphism
  - It is also known as late binding.if the binding process carried out at the run time  is called late binding.
  -      Overriding-No of methods and function with same name in diffrent class.
  -      Virtual keyword-It is used with methods, properties, indexers, and events in a base class to indicate that the implementation of that member can be overridden by a derived class.
  -      Method Hiding/New keyword-You can completely hide the implementation of the methods of a base class from the derived class using the new keyword.
 
 - ### Example of overriding
 ``` c#
 class animal
{
    public virtual void print()
    {
        Console.WriteLine("dog live in Home");
    }
}
class Lion:animal
{
    public override void print()
    {
        Console.WriteLine("Lion live in Jungle");
    }
}
public class HelloWorld
{
    public static void Main(string[] args)
    {
       animal a=new Lion();
       a.print();
    }
}

 ```


