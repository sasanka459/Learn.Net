### Continue and Break State ment With if else
### Continue
- It means to skip the remaining statement inside the loop and transfers the control to the beginning of the loop.

### Break
- Terminates the loop immediately.

### example of  Break

``` C#
public class breakstatement
{
    public static void Main(string[] args)
    {
       Console.WriteLine("\nBreak Statement Example:");
        for (int i = 0; i < 10; i++)
        {
            if (i == 5)
            {
                Console.WriteLine("Breaking loop at i = 5");
                break; // Exit the loop
            }
            Console.WriteLine("Current i: " + i);
        }
    }
}
```

### example of  Continue

```C#
public class statement
{
    public static void Main(string[] args)
    {
        Console.WriteLine("\nContinue Statement Example:");
        for (int i = 0; i < 5; i++)
        {
            if (i == 2)
            {
                continue; // Skip the rest of this iteration
            }
            Console.WriteLine("Current i (after continue check): " + i);
        }
    }
}
```
