# C# Notes

### Variable

A **variable** stores a value that can change as the program executes. Before you can use a variable, you must declare its data type and name and then initialize it by assigning a value to it.

A **variable** is associated with a data type which defines the type of data which can be stored in a variable.


### Variable naming conventions

- Must begin with a letter or underscore.
- First letter of variable name cannot be a - digit.
eg:
- First
- first
- _first
- 1first not accepted.


### Data types in C#

The built-in **data types** are actually aliases for the data types defined by the Common Type System of .NET.

- char - 2 bytes of memory
- int - 4 bytes of memory
- float - 4 bytes of memory
- double - 8 bytes of memory
- bool - 1 byte of memory
- string - variable length.

### Types of Data types in C#

1. **Value types**
    - which directly contains value.

```csharp
int myInt1 = 10 ; // contains a value of 10.

```
2. **Reference types**
-- it does not maintain the data but it contains a reference to variables which are stored in the memory.

```csharp
String myStr1; // Does not contain a value.
```



### Initializing a variable with a data type

#### syntax:

```csharp
// <datatype><variablename>=<value>;
eg:
int num1=45;

Console.WriteLine(num1); //45
Console.WriteLine("Number is {0}",num1); // Number is 45

char ch1='C';
Console.WriteLine(ch1); //C
Console.WriteLine("Character is {0}",ch1);

Console.WriteLine("Number is {0}\t Character is {1} ",num1,ch1);
Console.WriteLine("{0} {1}",num1,ch1);
float f1=333.4454F;
double d1=4454565666.432343645754754;
string str1="welcome to c#";
```
### Declare a variable with a data type

#### syntax:

```csharp
// <datatype><variablename>;
eg:
int num1;
char ch1;
float f1;
double d1;
string str1;

To Accept the value from the user use the method Console.ReadLine().
Console.ReadLine() accepts string data by default.

int - Convert.ToInt32()
char - Convert.ToChar()
float - Convert.ToSingle()
double - Convert.ToDouble()
bool - Convert.ToBoolean() or Convert.ToBool()

//Accept
Console.WriteLine("Enter a number");
num1=Convert.ToInt32(Console.ReadLine());
//Display
Console.WriteLine("number is {0}",num1);
```
