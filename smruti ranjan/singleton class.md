# Singleton Class
* ####  ***A singleton class is a blueprint in c# that restricts the initiation of more than one object in a class and it also provides global access of that object***
* Singleton Class uses private constuctor as default. To prevent create other as of that class out side the singleton class.
* It is gennerally used when we want to keep an object constant throughout the code.(ex- universal truths, credentials that dont ever change ,company name and details etc.)
## EXAMPLE

``` C#
using System;

public class log
{
    private static log a = null;
    private static readonly object padlock = new object();
    private log()
    {
        Console.WriteLine("log a created.");
    }
    
    public static log a
    {
        get
        {
            lock (padlock)
            {
                if (a == null)
                {
                    a = new log();
                }
                return a;
            }
        }
    }

    public void Log(string message)
    {
        Console.WriteLine("Log: " + message);
    }
}
```
