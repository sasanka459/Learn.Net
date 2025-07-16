### CLASS
- Class is a blueprint of object.it means calss can contains Constructors,method , properties and fields.
- The default access modifier of a class is internal.

### Nested classes (classes declared inside another class):
- The default access modifier is private.

### Object
- It is an instance of a class.



### example of class

```C#
class car
{
    private string carname;    //private field
    public int model;         //field
    public string Carname     //convert private field to public because we can access in another calss
    {
        get{return carname;}
        set{carname=value;}
    }
}
public class HelloWorld
{
    public static void Main(string[] args)
    {
       car c=new car();       //create calss object(c is the object of the car calss)
       c.Carname="suzuki";    //declar the value
       c.model=2024;
       Console.WriteLine(c.Carname);
       Console.WriteLine(c.model);
    }
}





