## Acess Modifiers

### Public

- If a class , field or method is decorated with `Public` modifiers. It will get acess in all the clases in the same assembly and in other assemblies

<details>
<Summary>Example</Summary>
 
 ```C#

 class PointTest
{
    public int x;
    public int y;
}

class Program
{
    static void Main()
    {
        var p = new PointTest();
        // Direct access to public members.
        p.x = 10;
        p.y = 15;
        Console.WriteLine($"x = {p.x}, y = {p.y}");
    }
}
// Output: x = 10, y = 15

 ```


</details>