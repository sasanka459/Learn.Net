## inheritance
-it is creating a parent and child relationship between two class where child class will autometically get the property of parent class.
-it provide the reusibility of cod and abstraction of code.
-it is 4 type:
1-single inheritance-it means there is one base class and one derive class.
2-multiple inheritance-c# does not support because of the Ambiguity function.
3-multilevel inheritance-when one class is derive from another derive class.
4-hierachical inheritance-when multiple class derived from one base class.

## example of inheritance

class car
{
  public void print1()
  {
      Console.WriteLine("suzuki");
  }
}
class model:car
{
    public void print2()
    {
        Console.WriteLine("2020");
    }
}
public class output
{
    public static void Main(string[] args)
    {
       model m=new model();
       m.print1();
       
    }
}


