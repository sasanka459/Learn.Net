## Abstraction
-it means the process of hiding implementation details and exposing only the essential features of an object or functionality.
-it reduce the complexity of viewing the things,Avoide code duplication and increase reusiblity.

## Abstract Class
-when we use abstract class we using abstract keyword.
-You are not allowed to create an object in the abstract calss.
-When a non-abstract (concrete) class inherits from an abstract class, it must implement all inherited abstract members.The implementation of an abstract member in a derived class is done using the override keyword.
-An abstract class can contain abstract member like abstract methods, properties, indexers, or events.
 These members are declared using the abstract keyword and do not have an implementation (a method body) in the abstract class.
   
     ##example
          public abstract class Vehicle
          {
            public abstract void StartEngine(); // Abstract method - no body
            public abstract int NumberOfWheels { get; set; } // Abstract property - no implementation
           }

### example of abstract calss
'''c#

 public abstract class employee
{
    public abstract void print();
    public void name()
    {
        Console.WriteLine("gati");
    }
}
class employee1:employee
{
    public override void  print()
    {
        Console.WriteLine("gati is our employee");
    }
}
public class output
{
    public static void Main(string[] args)
    {
       employee e=new employee1();
       e.print();
       e.name();
    }
}
