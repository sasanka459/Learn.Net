### Class

- Class is a logical signature. It contains method , properties and fields
- The default acess modifier for class is `internal`

### Object

Object is an instance of a class. We can create n number of object from a class.


### Example

```C#
  internal  class Person
    {
         byte? _age;


        //Constructor
        public Person()
        {
            Console.WriteLine("Hi Person");   
        }

        public void setAge(byte age)
        {
            if (age > 125)
            {
                throw new Exception("Invalid age");
            }
            _age = age;
        }

        public required string name;           
        public  required string email;
        public Address? address=null;


        public void displayName()
        {

            Console.WriteLine($"Hello {name}");
        }

        public void details()
        {

            Console.WriteLine($"Name : {name}, age : {_age}, email:{email} , address : {address}");
        }
    }


```