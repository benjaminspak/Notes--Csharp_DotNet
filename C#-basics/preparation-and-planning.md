#### Problem solving steps

##### The 4 P's

- Prepare - This is where we understand and diagnose the problem.
- Plan - This is where we organize everything before acting.
- Perform - We simply put the plan into action.
- Perfect - This is when we check to see if what we made has solved the problem and consider how to make it better. We can use the Four P's again to make improvements.

```c#
class Program
{
    static void Main()
    {
        // Prompt user for minutes exercised
        // Add minutes exercised to total
        // Display total minutes exercised to the screen
        // Repeat until user quits
    }
}
```

#### Writing to the console

```c#
// Prompt user for minutes exercised 
System.Console.Write("Enter how many minutes you exercised: ");
```

#### Running the compiler

```
$ mcs Program.cs
```

+ When running the compiler the output will be saved as a '.exe' file.

#### Namespaces, classes, methods

+ Namespaces - make it so that was can have multiple classes with the same name; as long as they are in another namespace.
+ Classes - are unique to a namespace.
+ Method - is an extension of a class. Also known as a function.

+ Note: not mentioning a namespace is poor practice.

```c#
namespace Treehouse
{
    class Program
    {
        static void Main()
        {

        }
    }
}
```

+ You can further break down namespaces for greater partitioning such as: `namespace Treehouse.FitnessFrog`

#### Using directive

+ You can scope your code within a namespace and cut down on the amount of code required to call a call and method.

```c#
using system;  // Using directive

class Program
{
    static void Main()
    {
        System.Console.Write("Enter how many minutes you exercised: ");  // Without the using directive.
        Console.Write("Enter how many minutes you exercised: ");  // With the using directive.
    }
}
```