### Readonly variable

- Readonly fields can be created using readonly keyword.
- ReadOnly is a runtime constant.
- The value of readonly field can be changed.
- It can be used with static modifiers.
- In readonly fields, we can assign values in declaration and in the constructor part.

### Example of Readonly variable

``` C#
namespace ReadOnly
{
    class Program
    {
        readonly int number;  //readonly variable
        //Initialize Readonly Variable through constructor
        public Program(int num)
        {
            number = num;
        }
        
        static void Main(string[] args)
        {
            Program obj1 = new Program(100);
            Console.WriteLine(obj1.number);

            //You cannot change the value of a readonly variable once it is initialized
            //The following statement will give us compile time error 
            //obj1.number = 20;

            Program obj2 = new Program(200);
            Console.WriteLine(obj2.number);
            Console.ReadLine();
        }
    }
}

 ```