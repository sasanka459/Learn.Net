# Pyramid Pattern
```c#
using System;
namespace MyApp
{
    class PyramidPattern
    {
        public static void Main()
        {
            Console.WriteLine("Enter The Height Of Pyramid:");
            int n = Convert.ToInt16(Console.ReadLine());

            for(int i=1; i<=n;i++)
            {
                for (int j = 1; j < n - i + 1; j++)
                { 
                    Console.Write(" ");
                }
                   
                
                for (int k = 1; k <= i; k++)
                    {
                    Console.Write("*");
                    Console.Write(" ");

                }
                Console.WriteLine();    
            }
        }
    }
}   
```
# Inverted Pyramid Pattern
```c#

using System;
namespace MyApp
{
    class InvertedPyramidPattern
    {
        public static void Main()
        {
            Console.WriteLine("Enter The Height Of Pyramid:");
            int n = Convert.ToInt16(Console.ReadLine());

            for (int i = n; i >=1; i--)
            {
                for (int j = 1; j < n - i + 1; j++)
                {
                    Console.Write(" ");
                }


                for (int k = 1; k <= i; k++)
                {
                    Console.Write("* ");
                }
                Console.WriteLine();
            }
        }
    }
}

```
# hollow Pyramid Pattern
```c#
using System;

namespace MyApp
{
    class HollowPyramid
    {
        public static void Main()
        {
            Console.Write("Enter the height of the pyramid: ");
            int n = Convert.ToInt32(Console.ReadLine());

            for (int i = 1; i <= n; i++)
            {
               
                for (int j = 1; j <= n - i; j++)
                {
                    Console.Write(" ");
                }

                // Print stars and hollow spaces
                for (int k = 1; k <= (2 * i - 1); k++)
                {
                    if (k == 1 || k == (2 * i - 1) || i == n)
                        Console.Write("*");
                    else
                        Console.Write(" ");
                }

                Console.WriteLine();
            }
        }
    }
}



```
# Diamond Pattern
```c#
using System;

namespace MyApp
{
    class DiamondPattern
    {
        public static void Main()
        {
            Console.Write("Enter the height of the pyramid: ");
            int n = Convert.ToInt32(Console.ReadLine());

            for (int i = 1; i <= n; i++)
            {
               
                for (int j = 1; j <= n - i; j++)
                {
                    Console.Write(" ");
                }

                // Print stars and hollow spaces
                for (int k = 1; k <= (2 * i - 1); k++)
                {
                    if (k == 1 || k == (2 * i - 1) )
                        Console.Write("*");
                    else
                        Console.Write(" ");
                }
                Console.WriteLine( );
                
            }
            for (int i = n-1 ; i >=1; i--)
            {

                for (int j = 1; j <= n - i; j++)
                {
                    Console.Write(" ");
                }

                
                for (int k = 1; k <= (2 * i - 1); k++)
                {
                    if (k == 1 || k == (2 * i - 1) )
                        Console.Write("*");
                    else
                        Console.Write(" ");
                }
                Console.WriteLine();

            }
        }
    }
}



```