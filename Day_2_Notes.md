# **C# Notes**

## .Net Framework Ecosystem

*The list items provided describe various components and technologies within the .Net Framework ecosystem, particularly focusing on C# and related frameworks for developing different types of applications.*

### **C#**:
   C# is a programming language used in the .Net Framework ecosystem. It is versatile and widely used for developing a variety of applications.

   - **Console Application (CUI)**: This refers to creating text-based applications that run in the command-line interface (terminal) and interact with the user through text input and output.

   - **Windows Forms (GUI)**: This involves building graphical desktop applications with user interfaces using Windows Forms, allowing developers to create interactive windows-based applications.

   - **Web Forms (GUI) (Asp.Net)**: Web Forms is a part of Asp.Net, which enables developers to create web applications with a drag-and-drop interface for building the user interface.

   - **ADO.Net**: ADO.Net stands for ActiveX Data Objects. It is a technology that allows .Net applications to access and interact with data sources, typically used for database access.

   - **MS SQL Server (Database)**: This refers to Microsoft SQL Server, a relational database management system, where data can be stored and manipulated.

### **Entity Framework**:
   Entity Framework (EF) is an Object-Relational Mapping (ORM) framework in the .Net ecosystem that simplifies database interactions by allowing developers to work with relational databases using object-oriented code.

   - **Asp.Net MVC**: ASP.Net MVC (Model-View-Controller) is a web application framework that separates application concerns into three components: model, view, and controller.

   - **Asp.Net Web Api + Angular/ReactJS**: This combination involves building web APIs using Asp.Net and creating frontend web applications using popular JavaScript frameworks/libraries like Angular or ReactJS.

### **Entity Framework Core**:
   Entity Framework Core is a lightweight and cross-platform version of Entity Framework, designed for .Net Core applications.

   - **Asp.Net Core MVC**: Similar to Asp.Net MVC, this is a web application framework for Asp.Net Core that follows the Model-View-Controller pattern.

   - **Asp.Net**: Asp.Net Core is a framework for building modern web applications and services.

   - **Web Api + Angular/ReactJS**: This combination is used for creating web APIs with Asp.Net Core and building frontend applications using Angular or ReactJS.

### <center>Console Application Example:</center>

```csharp
       // C# Program Structure

using System; // namespace 
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Day_2_ConsoleApp2 
{
    internal class Class1 // class
    {
        public static void Main(string[] args) // Main Method
        {
            // Code block 
            Console.WriteLine("Hi \tGuys! \n\"Welcome\" to \'C#\' class.");
            Console.ReadLine();
        }
    }
}
```
**<center>Summary</center>**

*Overall, the list outlines the various technologies and frameworks available within the .Net ecosystem for developing console applications, desktop applications, web applications, and web APIs, using C# as the primary programming language.*

## Escape Characters in C#:

*Escape characters in C# are special sequences used in strings to represent characters that are difficult or impossible to represent directly. They start with a backslash `\` followed by a specific character, and when included in a string, they produce a special behavior.*

Here is a chart with some commonly used escape characters in C#:

| Escape Character | Description                   | Example in C#          |
|------------------|-------------------------------|------------------------|
| `\n`               | Newline                       | `string text = "Hello\nWorld";` |
| `\t`               | Tab                           | `string text = "Hello\tWorld";` |
| `\r`               | Carriage return               | `string text = "Hello\rWorld";` |
| `\\`               | Backslash                     | `string text = "C:\\path\\to\\file";` |
| `\'`               | Single quote                  | `string text = "It\'s raining.";` |
| `\"`               | Double quote                  | `string text = "She said, \"Hello!\"";` |
| `\b`               | Backspace                     | `string text = "Hello\bWorld";` |
| `\a`               | Alert (bell)                  | `string text = "Alert! \a";` |

### <center>Escape Character Examples:</center>

```csharp
// Newline and Tab
string poem = "Roses are red,\nViolets are blue.\n\tSugar is sweet,\n\tAnd so are you.";

// Backslash
string filePath = "C:\\path\\to\\file";

// Single quote
string sentence = "I said, 'Hello!'";

// Double quote
string dialogue = "She replied, \"Sure, I'll come.\"";

// Backspace
string countDown = "5... 4... 3...\b\b2... 1...";

// Alert (bell)
Console.WriteLine("Hello! \a");
```

**<center>Summary</center>**

*In these examples, the escape characters are used to create newlines, tabs, show quotes within strings, create backslashes, create backspace effects, and produce alert sounds. These escape characters allow developers to handle special characters and formatting within strings effectively.*
