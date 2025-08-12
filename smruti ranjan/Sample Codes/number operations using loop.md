# Prime Nubers
``` C#
using System;
namespace MyApp
{
    class PrimeNumber
    {
        public static void Main()
        {
            Console.WriteLine("Enter The Number:");
            int n = Convert.ToInt16(Console.ReadLine());

            if (n <= 1)
            {
                Console.WriteLine(n + " is not a prime number");
                return;
            }

            bool isPrime = true;
            for (int i = 2; i <= Math.Sqrt(n); i++)
            {
                if (n % i == 0)
                {
                    isPrime = false;
                    break;
                }
            }

            if (isPrime)
            {
                Console.WriteLine(n + " is a prime number");
            }
            else
            {
                Console.WriteLine(n + " is not a prime number");
            }
        }
    }
}
```  
# Palindrome
```C#
using System;
namespace MyApp
{
    class NumericalPalindrome
    {
        public static void Main()
        {
            Console.WriteLine("Enter The Number:");
            int n = Convert.ToInt16(Console.ReadLine());

            int original = n;
            int reversed = 0;
             
            while (n>10)
            {
                int lastDigit = n % 10;
                reversed = reversed * 10 + lastDigit;
                n = n / 10;
            }
        if (original == reversed)
            {
                Console.WriteLine(original+" is a palindrome");
            }
        else Console.WriteLine(original+" is not a palindrome");
        }
    }
}

```
# Palindrome Using string
```
using System;
namespace MyApp
{
    class PalindromeChecker
    {
        public static void Main()
        {
            Console.Write("Enter A Word Or Number:");
            string word = Console.ReadLine();

            string wordString = word.ToLower();// Convert the input to lowercase for case-insensitive comparison

            char[] converted = wordString.ToCharArray();// Convert the string to a character array.
            Array.Reverse(converted);// Reverse the character array.
            string reversed = new string(converted);// Convert the reversed character array back to a string.
            if (reversed==wordString)
                {
                Console.WriteLine(word+ " : The word or number is a palindrome.");
            }
            else
            {
                Console.WriteLine(word+" : The word or number is not a palindrome.");
            }
            {
                
            }

        }
    }
}

```

# Fibbonacci Sequence
```
using System;
namespace MyApp
{
    class PalindromeChecker
    {
        public static void Main()
        {
            Console.Write("Enter A Word Or Number:");
            int num = Convert .ToInt16 (Console.ReadLine());

            int first = 0, second = 1, next;
            Console.Write("fibbonacci series:  ");
            for(int i=0;i<=num;i++)
            {
                next = first + second;
                first = second;
                second = next;
                Console.Write(next+", ");
            }



        }
    }
}

```
