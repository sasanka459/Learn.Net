# Properties
* In C# properties are members of a class that provide a flexible way to read, write, or compute the value of a field.
* We use properties to 
	> protect fields from invalid data(By using custom logic inside the properties).

	> validate data 

	>how data is accessed and modified.

 ## Types of Properties
  
 <details><summary> Getter & Setter({get; set;})</summary>

* It is a both read and write function i.e. we can insert data into a field and access tht data aswell.
* usually used to write & read data in a private field.
* It is a default property of c#.	

 ### EXAMPLE
```
private string _name;

public string Name
{
    get { return _name; }
    set { _name = value; }
}

Person p = new Person();
p.Name = "Smruti           // we use this to Write the name of the person p into memory(set).
Console.WriteLine(p.Name);     // We use this line to read the name of the same person from the memory(get).

output : Smruti

```
	
</details>

 <details><summary> Getter ({get;})</summary>

 * It is used in specific cases, where intitially the value of the private variable is assigned and it is not changed later.
 * Only read operations can be performed using this property.
 
 ### EXAMPLE
 ```
 private int _id = 1001;

public int ID
{
    get { return _id; }
}

Console.WriteLine(p.ID); 
Output:  2001
```

 </details>

 <details><summary>setter({set;})</summary>

* It is used in specific cases, where a data is only writen into the memory and its access should be  secure or private.
* Only Write operations can be performed using this property.
* Generally used to store passwords or sensetive info .

### EXAMPLE
```C#
private string _password;

public string Password
{
    set { _password = value; }
}

o.passwod = "secret";   // Password is writen into the memory and can't be accessed.
```


</details> 

 <details><summary>init ({get; init;}) </summary>

* It is very similar to the set property but in "init" proerty the value can only be assigned during initialization.
* The value cant be changed once its been initialized.
* "init" property is a relatively new property ,it was introduced in C# 9.0 which came out in nov 2020.

### EXAMPLE
```
public class Person
{
    public string Name { get; init; }
    public int Age { get; init; }
}

var p = new Person { Name = "Ranjan" , age= 25} //values assigned during initialization

Console.WriteLine(p.name);
Console.WriteLine(p.age);

output: ranjan
        25
```

 </details>

 <br>
  <br>
   <br>

 > We can also use custom ***get and set*** properties to restrict the input of invalid data. <br>
    **EXAMPLE** <br>


``` 
private int _age;
public int Age
{
    get { return _age; }
    set
    {
        if (value > 0 && value < 150)
            _age = value; // valid age ranging from 0 to 150 will be accepted.
        else
            Console.WriteLine("Invalid age"); // age outside the range will not be accepted.
    }
}
```