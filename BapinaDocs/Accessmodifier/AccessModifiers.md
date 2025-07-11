## AccessModifiers
-it is use to accessibility of a class.
-it is use to implement the encapsulation.
-AccessModifiers are 5 types.

1-Public:--The code is accessible for all classes.whether it's in the same assembly or a different one.

### example of public

```C#
public class calculator
{
    public int add(int a,int b)
    {
     return a+b;   
    }
    public static void Main(string[] args)
    {
      calculator c=new calculator();
      int result=c.add(10,20);
      Console.WriteLine(result);
    }
}

2-Private--Accessible only within the class.we can not access outside the class.
            

  class car
{
    private string carname;  //private 
    public int model;
    public string Carname    //convert private to public to access out side the class
    {
        get{return carname;}
        set{carname=value;}
    }
}
public class cars
{
    public static void Main(string[] args)
    {
       car c=new car();
       c.Carname="suzuki";
       c.model=2024;
       Console.WriteLine(c.Carname);
       Console.WriteLine(c.model);
    }
}

3-protected--Accessible from within the same class where it's declared AND from derived classes (classes that inherit from it).
    

4-internal--Accessible from anywhere within the same assembly (e.g., the same project or .dll file). Not accessible from other assemblies.

5-protected internal--Accessible within the same assembly OR by derived classes
