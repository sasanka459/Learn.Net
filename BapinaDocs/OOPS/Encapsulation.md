### Encapsulation

- The process of binding the data and function together into a single unit .
- We can implement encaplution:-by declaring the variable as private,by using access modifier
- Using accessor(get method) and mutator (set method) methods we can make encapsulation
- We can use encapsulation To Protect Sensitive Data,When You Need to Add Validation(Validating user input, such as ensuring that a product price cannot be negative or a username cannot be blank.),To Hide Implementation Details.
- Where to Use- Use Encapsulation(In Large-Scale Applications,When Designing APIs or Libraries,To Enforce Business Rules,In Security-Critical Applications).

### example of Encapsulatio
```c#
class bank
{
 private string Name;
 public string name
 {
     get{return Name;}
     set{Name= value;}
 }
}
public class HelloWorld
{
    public static void Main(string[] args)
    {
      bank b=new bank();
      b.name="gati";
      Console.WriteLine(b.name);
    }
}
```






