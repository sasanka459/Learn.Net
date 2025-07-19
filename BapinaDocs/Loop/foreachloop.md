### Foeeach Loop
- It run through items in collection or  It is used to iterate over elements of a collection (like arrays, lists, etc.) or other enumerable objects.

### Syntax

```C#
foreach (type variableName in collection)
{
    // code to be executed
}
```

### Example of Foreach Loop

``` C#
public class Cars
{
    public static void Main(string[] args)
    {
       string[] cars={"suzuki","audi","Volvo", "BMW", "Ford"};
       foreach(string i in cars)
       {
           Console.WriteLine("cars name are: "+i);
       }
    }
}
```
