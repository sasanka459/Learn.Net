### While Loop
- The while loop loops through a block of code as long as a specified condition is True.

### syntax

```C#
while (condition) 
{
  // code block to be executed
}
```

### Example Of WhileLoop

```C#
 class whileloop
  {
    static void Main(string[] args)
    {
      int i = 0;
      while (i < 5) 
      {
        Console.WriteLine(i);
        i++;
      }
    }
  }
```

### Do While Loop
- This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

### Syntax

```C#
do 
{
  // code block to be executed
}
while (condition);
```

### Example of Do while loop

```C#
class dowhileloop
  {
    static void Main(string[] args)
    {
      int i = 0;
      do 
      {
        Console.WriteLine(i);
        i++;
      }
      while (i < 5);
    }
  }

```