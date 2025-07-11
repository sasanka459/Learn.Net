## forloop
-it run through the items until the execution condition is true.
-when you run forloop 1st it goes to initialization then  condition then Increment or Decrement.

-for (initialization; condition; iterator)
{
    // Code to be executed repeatedly
}

### example of forloop

```C#
public class Reverse
{
    public static void Main(string[] args)
    {
      Console.WriteLine("Enter your string: ");
        string org=Console.ReadLine();
        string rev=" ";
        for(int i=org.Length-1;i>=0;i--)
        {
            rev+=org[i];
        }
        Console.WriteLine("Reverse string is : "+rev);
    }
}