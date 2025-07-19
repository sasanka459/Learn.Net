### Constant Variable

- In C#, constant fields are created using const keyword.
- Const is a compile time constant.
- The value of the const field can not be changed.
- It cannot be used with static modifiers.
- In const fields, we can only assign values in declaration part.

### Example of Constant variable 

``` C#
namespace Constvariable
{
    class Program
    {
        const float PI = 3.14f; //Constant Variable
        static void Main(string[] args)
        {
            //Const variables are static in nature
            //so we can access them by using class name 

            Console.WriteLine(Program.PI);

            //We can also access them directly within the same class

            Console.WriteLine(PI);

            //We can also declare a constant variable within a function

            const int Number = 10;
            Console.WriteLine(Number);

            //Once after declaration we cannot change the value 
            //of a constant variable. So, the below line gives an error
            //Number = 20;
            Console.ReadLine();
        }
    }
}
```