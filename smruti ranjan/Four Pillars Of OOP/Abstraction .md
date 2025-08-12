# **ABSTRACTION**
* Abstaction  hides the complex implementation details and only shows the essential features of an object or system.
* Abstract keyword is used before a class or method to implement Abstaction.
* Override keyword is used in the child class.
* Abstract class can have abstract methods .
* abstract methods cant have a body of codes.


## EXAMPLES
```C#
abstract class Payment
{
    public abstract void Processing(); 
}


class CardPayment : Payment
{
    public override void Processing()
    {
       
        Console.WriteLine("Validating card");
        Console.WriteLine("Processing credit card payment");
    }
}


class Program {
    static void Main() {
        Payment payment = new CardPayment();
        payment.Processing();
     
    }
}
OUTPUT : 
        Validating card
        Processing credit card payment

```