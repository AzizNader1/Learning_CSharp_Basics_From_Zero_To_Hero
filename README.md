# Master C# Programming Basics: Complete A to Z Guide

> **From Zero to Hero: Learn C# Fundamentals from the Ground Up**

---

## Table of Contents

1. [Introduction to C# and .NET](#1-introduction-to-c-and-net)
2. [Setting Up Your Development Environment](#2-setting-up-your-development-environment)
3. [Program Structure and Basic Syntax](#3-program-structure-and-basic-syntax)
4. [Variables and Data Types](#4-variables-and-data-types)
5. [Type Conversion and Casting](#5-type-conversion-and-casting)
6. [Operators in C#](#6-operators-in-c)
7. [Control Flow Statements](#7-control-flow-statements)
8. [Loops and Iteration](#8-loops-and-iteration)
9. [Arrays](#9-arrays)
10. [Methods (Functions)](#10-methods-functions)
11. [String Manipulation](#11-string-manipulation)
12. [Exception Handling Basics](#12-exception-handling-basics)
13. [Console Input and Output](#13-console-input-and-output)
14. [Collections: List and Dictionary](#14-collections-list-and-dictionary)
15. [Enumerations (Enums)](#15-enumerations-enums)
16. [Structs](#16-structs)
17. [Basic File Operations](#17-basic-file-operations)
18. [Best Practices for Beginners](#18-best-practices-for-beginners)

---

## 1. Introduction to C# and .NET

### What is C#?

C# (pronounced "C Sharp") is a modern, object-oriented programming language developed by Microsoft as part of the .NET initiative in the early 2000s. Designed by Anders Hejlsberg and his team, C# was created to be a simple, modern, general-purpose, and object-oriented language that would address many of the complexities and issues found in languages like C++ and Java. The name "C Sharp" was inspired by the musical notation where a sharp symbol indicates that a note should be made higher in pitch—symbolizing that C# is an enhancement of C++.

C# is a strongly-typed language, meaning that every variable and expression has a type that is known at compile time. This characteristic helps catch errors early in the development process, before the code is even run. The language is designed to be type-safe, ensuring that variables can only contain values appropriate to their type, which prevents many common programming errors and security vulnerabilities. C# also incorporates automatic memory management through garbage collection, freeing developers from the burden of manual memory allocation and deallocation that plagues languages like C++.

### Understanding the .NET Ecosystem

To understand C# properly, you must first understand the .NET platform on which it runs. .NET is a development platform that provides a controlled environment for developing and executing applications. It includes a runtime environment called the Common Language Runtime (CLR) and a comprehensive class library called the Base Class Library (BCL). The CLR handles memory management, security, and exception handling, while the BCL provides pre-built code for common programming tasks like file I/O, database access, and web development.

The evolution of .NET has been significant over the years. Originally, there was the .NET Framework, which ran only on Windows. Later, Microsoft introduced .NET Core as a cross-platform, open-source successor. Today, the platform has unified under the name ".NET" (dropping "Core"), with versions like .NET 6, .NET 7, and .NET 8 providing consistent APIs across Windows, Linux, and macOS. This cross-platform capability has dramatically expanded C#'s reach, making it viable for developing applications that run on any operating system, from web servers to mobile devices to cloud services.

### Why Learn C#?

C# consistently ranks among the most popular and widely-used programming languages worldwide, and there are compelling reasons for its sustained popularity. First, C# is incredibly versatile—it can be used to build virtually any type of application, including desktop applications (Windows Forms, WPF), web applications (ASP.NET), mobile applications (Xamarin, now part of .NET MAUI), games (Unity), cloud services (Azure), and even IoT devices. This versatility means that learning C# opens doors to numerous career paths and project types.

The language also benefits from excellent tooling, particularly Visual Studio and Visual Studio Code, which provide world-class development experiences including intelligent code completion (IntelliSense), powerful debugging capabilities, and integrated testing tools. Microsoft's commitment to the language is evident in its continuous evolution—new versions of C# are released regularly, introducing modern language features that improve developer productivity and code expressiveness. Additionally, the .NET ecosystem includes extensive documentation, a large community of developers, and a wealth of third-party libraries available through NuGet, the package manager for .NET.

### C# vs Other Languages

When comparing C# to other programming languages, several distinctions become apparent. Compared to C++, C# provides higher-level abstractions and automatic memory management, making it easier to write safe code, though at the cost of some low-level control. Compared to Java, C# offers similar object-oriented features but includes more modern language constructs like properties, events, and LINQ (Language Integrated Query). Compared to Python, C# is statically typed and compiled, which means better performance and earlier error detection, but potentially more verbose code.

For beginners, C# offers an excellent learning path because it enforces good programming practices while remaining accessible. The strongly-typed nature of the language teaches important concepts about data types and program structure. The syntax is clean and consistent, borrowing the best elements from C-style languages while avoiding some of their pitfalls. As you progress from basics to advanced topics, C# scales well—professional developers use the same language for everything from simple scripts to enterprise-scale systems serving millions of users.

---

## 2. Setting Up Your Development Environment

### Installing Visual Studio

The most comprehensive development environment for C# is Visual Studio, Microsoft's flagship integrated development environment (IDE). Visual Studio Community Edition is free for individual developers, open-source projects, academic research, and small professional teams, making it accessible for learners and professionals alike. The installation process is straightforward: download the installer from the Microsoft website, run it, and select the workloads you need for your development tasks.

During installation, you'll be presented with various workloads—pre-configured sets of features for different development scenarios. For learning C# basics, select the ".NET desktop development" workload, which includes everything needed for console applications and desktop development. If you're interested in web development, add the "ASP.NET and web development" workload. The installation may take some time depending on your internet speed and selected components, as Visual Studio is a substantial application with many features.

After installation, when you first launch Visual Studio, you'll be prompted to sign in with a Microsoft account. While optional, signing in allows you to synchronize your settings across multiple machines and access additional services. You'll also be asked to choose your development settings—select "General" or "Visual C#" for the most relevant defaults. The start page provides quick access to recent projects, the ability to create new projects, and access to documentation and tutorials.

### Installing Visual Studio Code (Lightweight Alternative)

If you prefer a lighter-weight development environment, Visual Studio Code (VS Code) is an excellent alternative. VS Code is a free, open-source code editor developed by Microsoft that has become incredibly popular among developers. While less feature-rich than the full Visual Studio IDE, VS Code is faster, more customizable, and works well for learning C#. To set up VS Code for C# development, you'll need to install the C# Dev Kit extension, which provides language support, debugging, and project templates.

The setup process for VS Code involves several steps. First, download and install VS Code from the official website. Then, install the .NET SDK separately from the .NET website—this provides the compilers and runtime needed to build and run C# applications. Finally, open VS Code and install the C# extension (or C# Dev Kit for a more complete experience). This extension provides IntelliSense, debugging support, and other productivity features. VS Code's lightweight nature makes it ideal for quick coding sessions and learning exercises.

### Installing the .NET SDK

Regardless of which editor or IDE you choose, you need the .NET Software Development Kit (SDK) installed on your machine. The SDK includes the compilers (C# compiler is called Roslyn), the .NET runtime, and the command-line tools needed to build and run applications. You can download the SDK from the official .NET website—select the version that matches your operating system. As of this writing, .NET 8 is the latest Long Term Support (LTS) version, recommended for most users.

To verify your installation, open a command prompt or terminal and run the following command:

```bash
dotnet --version
```

This command should display the installed .NET SDK version. If you see an error message instead, the SDK may not be installed correctly or may not be in your system's PATH. The `dotnet` command-line interface (CLI) is a powerful tool for creating, building, and running .NET applications from the command line, and you'll use it extensively throughout your C# journey.

### Creating Your First Project

Let's create your first C# project using the command line. Open a command prompt or terminal, navigate to a directory where you want to store your projects, and run these commands:

```bash
# Create a new console application
dotnet new console -n MyFirstApp

# Navigate into the project directory
cd MyFirstApp

# Run the application
dotnet run
```

The `dotnet new console` command creates a new console application project with a basic structure. The `-n` flag specifies the project name. The `dotnet run` command compiles and executes your application in one step. You should see "Hello, World!" printed to the console, which is the default output of a new console application.

The project structure created by these commands includes:
- **Program.cs**: The main source code file containing your application's entry point
- **MyFirstApp.csproj**: The project file that defines project settings and dependencies
- **obj/** and **bin/** directories: Contain compiled outputs and intermediate files (created after first build)

---

## 3. Program Structure and Basic Syntax

### Understanding Program.cs

In C#, every application starts execution from a specific entry point. For console applications, this entry point is traditionally a method called `Main`. The structure of Program.cs has evolved significantly over the years, with modern C# (version 9 and later) supporting "top-level statements" that simplify the code considerably. Let's examine both the traditional and modern approaches to understand how C# programs are organized.

**Traditional Program Structure (C# 8 and earlier):**

```csharp
using System;

namespace MyFirstApp
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
}
```

**Modern Program Structure (C# 9 and later - Top-level statements):**

```csharp
// This is all you need in modern C#!
Console.WriteLine("Hello, World!");
```

The modern approach with top-level statements is much simpler and ideal for learning. Behind the scenes, the compiler generates the necessary class and Main method boilerplate automatically. However, understanding the traditional structure is important because you'll encounter it in existing codebases and documentation, and it helps you understand how C# programs are fundamentally organized.

### Namespaces and Using Directives

Namespaces in C# provide a way to organize code and prevent naming conflicts between different parts of a program or between different libraries. Think of namespaces as containers that hold related types (classes, structs, enums, etc.). The .NET framework itself is organized into numerous namespaces—for example, `System` contains fundamental types, `System.IO` contains input/output types, and `System.Collections` contains collection types.

The `using` directive imports namespaces so you can use the types they contain without fully qualifying them. For example, without `using System;`, you would need to write `System.Console.WriteLine()` instead of just `Console.WriteLine()`. Multiple using directives typically appear at the top of a file:

```csharp
using System;
using System.IO;
using System.Collections.Generic;

// Your code here can now use types from these namespaces directly
```

Starting with C# 10, you can use implicit usings, which automatically include common namespaces without explicitly writing them. This feature is enabled by default in modern .NET project templates, which is why new console applications might not show any using directives at all yet still have access to common types like `Console` and `DateTime`.

### Comments and Documentation

Comments are essential for making your code understandable to yourself and others. C# supports three types of comments: single-line comments, multi-line comments, and documentation comments. Using comments appropriately is a key skill for writing maintainable code, though the best code is self-documenting through clear naming and structure.

```csharp
// This is a single-line comment
// It starts with two forward slashes and extends to the end of the line

/*
 * This is a multi-line comment
 * It can span multiple lines
 * and is useful for longer explanations or temporarily disabling code
 */

/// <summary>
/// This is a documentation comment (XML documentation)
/// It can be used to generate API documentation
/// and provides IntelliSense information in Visual Studio
/// </summary>
/// <param name="name">The name of the person to greet</param>
/// <returns>A greeting message</returns>
public string Greet(string name)
{
    return $"Hello, {name}!";
}
```

Single-line comments are most common for brief explanations or notes. Multi-line comments are useful when you need to write longer explanations or temporarily disable a block of code during debugging. Documentation comments use XML tags and can be processed by tools to generate documentation websites or provide rich IntelliSense information in the IDE. While you may not write extensive documentation as a beginner, understanding these comment types helps you read and understand existing code.

### Statements and Expressions

A fundamental concept in C# programming is the distinction between statements and expressions. Understanding this distinction helps you reason about how programs work and how to construct them correctly. An expression is any combination of values, variables, operators, and method calls that produces a value. A statement is a complete instruction that the compiler can execute—it performs an action but doesn't necessarily produce a value.

```csharp
// Examples of expressions (they produce a value):
5                           // Literal value expression
x + 10                      // Arithmetic expression
Math.Sqrt(16)               // Method call expression
x > 0                       // Boolean expression
"Hello" + " World"          // String concatenation expression

// Examples of statements (they perform an action):
int x = 10;                 // Declaration statement with initialization
Console.WriteLine("Hi");    // Expression statement (method call)
if (x > 0) { ... }          // If statement
return x + 1;               // Return statement

// Statements end with semicolons in C#
int result = 5 + 3;         // The whole line is a statement
                           // (5 + 3) is an expression within it
```

Every C# program consists of a series of statements that execute in sequence (unless control flow statements change the order). Statements are terminated with semicolons, which tell the compiler where one statement ends. Forgetting semicolons is one of the most common errors for beginners—always check for missing semicolons if you see unexpected syntax errors.

### Code Blocks and Scope

A code block is a group of statements enclosed in curly braces `{ }`. Code blocks define scope—the region of code where a variable or other named element is accessible. Variables declared inside a code block are only accessible within that block and its nested blocks. Understanding scope is crucial for organizing your code and avoiding errors related to variable visibility.

```csharp
int outerVariable = 10;     // Accessible throughout the method

if (outerVariable > 5)
{
    // This is a code block
    int innerVariable = 20; // Only accessible inside this block
    Console.WriteLine(outerVariable);  // OK - outerVariable is in scope
    Console.WriteLine(innerVariable);  // OK - innerVariable is in scope
}

Console.WriteLine(outerVariable);      // OK - still in scope
// Console.WriteLine(innerVariable);   // ERROR! innerVariable is out of scope
```

The concept of scope applies not just to code blocks within methods, but also to namespaces, classes, and methods themselves. A variable's scope begins at its declaration and ends at the closing brace of the block in which it's declared. This is why you can't use a variable before you've declared it, and why variables with the same name can exist in different scopes without conflict.

---

## 4. Variables and Data Types

### What are Variables?

Variables are fundamental building blocks in any programming language. A variable is a named storage location in computer memory that holds a value. Think of a variable as a labeled box where you can store data—once you've created the box and labeled it, you can put things in, take things out, and refer to it by name. In C#, variables must be declared with a specific type, which determines what kind of data the variable can hold and how much memory is allocated for it.

The process of creating a variable is called declaration. When you declare a variable, you tell the compiler its name and type. Optionally, you can also initialize the variable at the same time—give it an initial value. If you don't initialize a variable, its value is undefined (for local variables, you must assign a value before using them). The combination of declaration and initialization in one statement is the most common pattern.

```csharp
// Declaration only (variable must be assigned before use)
int age;

// Declaration with initialization (recommended)
string name = "John";

// Multiple declarations of the same type
int x, y, z;

// Multiple declarations with initialization
int a = 1, b = 2, c = 3;
```

### Value Types vs Reference Types

C# divides types into two main categories: value types and reference types. This distinction is fundamental to understanding how C# manages data and memory. Value types directly contain their data—a variable of a value type holds the actual value. Reference types store a reference to their data—the variable holds a memory address where the actual data is stored.

Value types include all numeric types (int, double, decimal, etc.), boolean (bool), character (char), and custom structs. When you assign one value type variable to another, a copy of the value is made. Changes to one variable don't affect the other. This is called value semantics and is intuitive for simple data types.

```csharp
int a = 10;
int b = a;      // b gets a copy of a's value
a = 20;         // changing a doesn't affect b
Console.WriteLine(a);  // Output: 20
Console.WriteLine(b);  // Output: 10
```

Reference types include strings, arrays, and all classes. When you assign one reference type variable to another, you're copying the reference, not the actual data. Both variables point to the same object in memory. Changes made through one variable are visible through the other. This is called reference semantics.

```csharp
int[] arr1 = { 1, 2, 3 };
int[] arr2 = arr1;    // arr2 now references the same array
arr1[0] = 99;         // modifying through arr1
Console.WriteLine(arr2[0]);  // Output: 99 (change visible through arr2)
```

Understanding this distinction becomes crucial when passing variables to methods, returning values from methods, and comparing values for equality. We'll explore these implications throughout this tutorial.

### Numeric Data Types

C# provides various numeric types to handle different kinds of numbers efficiently. Choosing the appropriate type depends on the range of values you need to store and whether you need decimal precision. Here's a comprehensive overview of the numeric types available:

**Integer Types (Whole Numbers):**

| Type | Size | Range | Usage |
|------|------|-------|-------|
| `sbyte` | 1 byte | -128 to 127 | Small signed integers |
| `byte` | 1 byte | 0 to 255 | Small positive numbers, raw data |
| `short` | 2 bytes | -32,768 to 32,767 | Small integers |
| `ushort` | 2 bytes | 0 to 65,535 | Small positive integers |
| `int` | 4 bytes | -2.1B to 2.1B | Most common integer type |
| `uint` | 4 bytes | 0 to 4.3B | Large positive integers |
| `long` | 8 bytes | Very large range | Large integers, file sizes |
| `ulong` | 8 bytes | 0 to very large | Very large positive integers |

**Floating-Point Types (Decimal Numbers):**

| Type | Size | Precision | Usage |
|------|------|-----------|-------|
| `float` | 4 bytes | ~7 digits | Scientific calculations |
| `double` | 8 bytes | ~15 digits | General decimal calculations |
| `decimal` | 16 bytes | ~28 digits | Financial calculations |

```csharp
// Integer literals
int population = 8000000000;
long bytesOnDisk = 5000000000000L;  // L suffix for long
uint positiveOnly = 4000000000U;    // U suffix for unsigned

// Floating-point literals
float temperature = 98.6f;          // f suffix for float
double pi = 3.14159265358979;       // default for decimal literals
decimal price = 19.99m;             // m suffix for decimal (money)
```

The `int` type is the default choice for whole numbers, as it provides a good balance between range and memory usage. For decimal numbers, `double` is the default and appropriate for most calculations. Use `decimal` for financial calculations where exact decimal representation is required—`float` and `double` can have small rounding errors that accumulate.

### Boolean Type

The `bool` type represents a Boolean value, which can be either `true` or `false`. Boolean values are fundamental to programming logic—they're used in conditional statements, loops, and anywhere you need to represent a yes/no, on/off, or true/false state. Unlike some languages that use integers for Boolean values (0 for false, non-zero for true), C# has a dedicated `bool` type, which makes code clearer and prevents certain types of errors.

```csharp
bool isStudent = true;
bool hasLicense = false;
bool isAdult = age >= 18;           // Result of comparison is bool
bool canVote = isAdult && hasId;    // Logical operations produce bool

// Common patterns using bool
if (isStudent)
{
    Console.WriteLine("Student discount applies!");
}

while (!isComplete)
{
    // Continue processing
}
```

Boolean variables are often named with prefixes like "is", "has", "can", or "should" to make their purpose clear. This naming convention makes code read more naturally: `if (isComplete)`, `while (hasMoreData)`, etc. You can also use nullable bool (`bool?`) when you need to represent three states: true, false, and unknown/null.

### Character Type

The `char` type represents a single Unicode character. A char occupies 2 bytes, allowing it to represent any character in the Unicode Basic Multilingual Plane. Characters are written using single quotes, distinguishing them from strings which use double quotes. The char type is the building block for text processing, and understanding it is essential for working with strings.

```csharp
char letter = 'A';
char digit = '7';
char symbol = '@';
char space = ' ';
char unicode = '\u0041';    // Unicode escape for 'A'

// Escape sequences for special characters
char newline = '\n';        // Newline
char tab = '\t';            // Tab
char backslash = '\\';      // Backslash
char singleQuote = '\'';    // Single quote

// Characters are actually numeric values
char c = 'A';
Console.WriteLine((int)c);  // Output: 65 (ASCII value)

// Character arithmetic
char nextLetter = (char)(c + 1);  // 'B'
```

Characters can participate in arithmetic operations because each character has a corresponding numeric code point. This enables techniques like converting between uppercase and lowercase letters, iterating through the alphabet, or validating character input.

### String Type

A string is a sequence of characters representing text. Strings in C# are reference types, but they behave somewhat uniquely—they're immutable, meaning once a string is created, it cannot be changed. Any operation that appears to modify a string actually creates a new string. This immutability has important implications for performance and behavior.

```csharp
// String declaration and initialization
string greeting = "Hello, World!";
string empty = "";
string alsoEmpty = string.Empty;  // Preferred for empty strings
string nullString = null;          // No string at all (different from empty)

// String with escape characters
string path = "C:\\Users\\John\\Documents";  // Escaped backslashes
string quote = "He said, \"Hello!\"";         // Escaped quotes

// Verbatim strings (preserve formatting, backslashes literal)
string verbatimPath = @"C:\Users\John\Documents";
string multiLine = @"This is
a multi-line
string";

// Raw string literals (C# 11+)
string json = """
    {
        "name": "John",
        "age": 30
    }
    """;
```

The distinction between an empty string (`""`) and a null reference is important. An empty string is a valid string with zero length. A null reference means the variable doesn't reference any string at all. Attempting to call methods on a null string causes a runtime error (`NullReferenceException`), so you should always check for null before using a string variable.

### Variable Naming Conventions

Choosing good names for variables is crucial for writing readable, maintainable code. C# has specific naming conventions that are widely followed in the .NET community. Following these conventions makes your code consistent with the framework and easier for other developers to understand.

```csharp
// Convention: camelCase for local variables and parameters
int studentAge = 20;
string firstName = "John";
bool isValidEmailAddress = true;
decimal totalPriceIncludingTax = 100.00m;

// Convention: PascalCase for methods, classes, and public properties
// (We'll cover these when we discuss OOP)

// Avoid these naming practices:
int x = 10;                    // Too short, not descriptive
int theVariableThatHoldsAge = 20;  // Too verbose
string name2 = "Jane";         // Numeric suffixes usually indicate poor naming
string mystring = "text";      // Doesn't follow casing convention
string MyString = "text";      // Wrong casing for local variable
```

Good variable names are descriptive enough to indicate purpose but concise enough to be readable. A variable's name should answer "what" it represents, not "how" it's used or "when" it changes. Single-letter names are acceptable only for loop counters (like `i`, `j`, `k`) or in very short, obvious contexts.

### Constants and Read-Only Variables

Sometimes you need variables whose values should never change after initialization. C# provides two mechanisms for this: constants (`const`) and read-only variables (`readonly`). Constants must be assigned a value at compile time and are implicitly static. Read-only variables can be assigned at runtime (in a constructor) but cannot be changed afterward.

```csharp
// Constants - value must be known at compile time
const double Pi = 3.14159265358979;
const int MaxRetries = 3;
const string ApplicationName = "MyApp";

// Constants are often named with PascalCase or ALL_CAPS
const int MAX_CONNECTIONS = 100;
const int DefaultTimeoutMs = 30000;

// Using constants
double circumference = 2 * Pi * radius;

// readonly - for values determined at runtime
// (Used in classes, covered in OOP)
public class Configuration
{
    public readonly string ApiKey;
    
    public Configuration(string apiKey)
    {
        ApiKey = apiKey;  // Can be set once in constructor
    }
}
```

Using constants improves code readability and maintainability. Instead of "magic numbers" scattered throughout your code, you have named constants that explain what the values represent. If you need to change a value, you change it in one place. Constants also prevent accidental modification, which can be a source of bugs.

---

## 5. Type Conversion and Casting

### Implicit Conversions

C# automatically converts between compatible types when the conversion is guaranteed to succeed without data loss. These implicit conversions happen automatically without any special syntax. The general rule is that implicit conversions are allowed when the target type can represent all possible values of the source type—typically when converting from a "smaller" type to a "larger" type.

```csharp
// Implicit numeric conversions
int intValue = 42;
long longValue = intValue;      // int fits in long - implicit conversion
double doubleValue = intValue;  // int fits in double - implicit conversion

// Implicit conversion chain
byte small = 100;
int medium = small;             // byte → int
long large = medium;            // int → long
double huge = large;            // long → double

// No syntax needed - conversion is automatic
Console.WriteLine(huge);        // Output: 100
```

Implicit conversions make code cleaner and are safe because the compiler can guarantee no data loss. The conversion happens at the moment of assignment. Understanding implicit conversions helps you write code that compiles and behaves correctly without unnecessary explicit casting.

### Explicit Conversions (Casting)

When you need to convert between types that might lose data, or between types that aren't automatically compatible, you must use explicit conversion, also called casting. Explicit conversions require you to acknowledge that data loss might occur by writing the target type in parentheses before the value being converted.

```csharp
// Explicit conversion with potential data loss
double pi = 3.14159;
int truncated = (int)pi;        // Explicit cast required
Console.WriteLine(truncated);   // Output: 3 (decimal portion lost)

long bigNumber = 5000000000L;
int overflow = (int)bigNumber;  // Explicit cast required
Console.WriteLine(overflow);    // Output: 705032704 (overflow occurred!)

// Casting reference types
object obj = "Hello";
string str = (string)obj;       // Cast object to string

// Casting can fail at runtime if types are incompatible
object num = 42;
// string invalid = (string)num;  // Runtime exception: InvalidCastException
```

When casting numeric types, be aware that data loss can occur in two ways: truncation (losing decimal places when converting floating-point to integer) and overflow (when the source value exceeds the target type's range). The compiler doesn't warn you about these possibilities—it assumes you know what you're doing when you explicitly cast.

### Using Convert Class

The `Convert` class provides methods for converting between various types with more control over the conversion process. Unlike casting, Convert methods can handle null values gracefully and provide consistent behavior across different conversion scenarios.

```csharp
// Convert to string
int number = 42;
string numberAsString = Convert.ToString(number);

// Convert from string
string numericString = "123";
int parsedNumber = Convert.ToInt32(numericString);
double parsedDouble = Convert.ToDouble("3.14");
bool parsedBool = Convert.ToBoolean("true");

// Handling null (Convert methods return default values)
object? nullValue = null;
int defaultValue = Convert.ToInt32(nullValue);  // Returns 0

// Converting between bases
string binary = Convert.ToString(10, 2);   // "1010" (binary)
string hex = Convert.ToString(255, 16);    // "ff" (hexadecimal)
int fromBinary = Convert.ToInt32("1010", 2);  // 10
```

The Convert class is particularly useful when dealing with string input that needs to be converted to numeric types, such as user input or data from text files. However, if the string can't be parsed as the target type, Convert methods throw an exception, so you should validate input or use parsing methods with error handling.

### Parsing Strings

When you need more control over converting strings to other types, or when you want to handle conversion failures gracefully, use the `Parse` and `TryParse` methods. These methods are available on all numeric types and other common types like DateTime and bool.

```csharp
// Parse method - throws exception on failure
string numberText = "42";
int parsed = int.Parse(numberText);        // Returns 42

// Parse with culture-specific formatting
string decimalText = "3,14";               // European decimal separator
var culture = new System.Globalization.CultureInfo("de-DE");
decimal value = decimal.Parse(decimalText, culture);

// TryParse method - returns success/failure without throwing
string input = "123";
if (int.TryParse(input, out int result))
{
    Console.WriteLine($"Successfully parsed: {result}");
}
else
{
    Console.WriteLine("Failed to parse the input");
}

// TryParse is ideal for user input
Console.Write("Enter your age: ");
string? ageInput = Console.ReadLine();
if (int.TryParse(ageInput, out int age) && age >= 0 && age <= 150)
{
    Console.WriteLine($"You are {age} years old.");
}
else
{
    Console.WriteLine("Please enter a valid age.");
}
```

The `TryParse` pattern is the recommended approach for handling user input or any string that might not be in the expected format. It returns a boolean indicating success or failure, and outputs the parsed value through an `out` parameter. This pattern avoids the performance overhead of exception handling for expected conversion failures.

### Boxing and Unboxing

Boxing is the process of converting a value type to a reference type (specifically, to `object` or an interface). Unboxing is the reverse—converting a boxed reference back to a value type. While this happens automatically in many contexts, understanding boxing helps you write more efficient code.

```csharp
// Boxing - value type to reference type
int value = 42;
object boxed = value;           // Implicit boxing

// Unboxing - reference type back to value type
int unboxed = (int)boxed;       // Explicit unboxing

// Boxing in action (ArrayList stores objects)
using System.Collections;
ArrayList list = new ArrayList();
list.Add(1);                    // int boxed to object
list.Add(2);                    // int boxed to object
list.Add(3);                    // int boxed to object

// Each retrieval requires unboxing
int sum = 0;
foreach (object item in list)
{
    sum += (int)item;           // Unboxing each item
}

// Generic collections avoid boxing
using System.Collections.Generic;
List<int> genericList = new List<int>();
genericList.Add(1);             // No boxing - stores int directly
int first = genericList[0];     // No unboxing needed
```

Boxing has performance implications—it allocates memory on the heap and involves copying the value. For this reason, generic collections like `List<T>` are preferred over non-generic collections like `ArrayList`, as they avoid boxing when storing value types. Understanding boxing helps you recognize performance issues in code that heavily uses the `object` type.

---

## 6. Operators in C#

### Arithmetic Operators

Arithmetic operators perform mathematical calculations on numeric values. C# supports the standard arithmetic operations you're familiar with from mathematics, plus some additional operators that combine assignment with arithmetic.

```csharp
int a = 10;
int b = 3;

// Basic arithmetic
int sum = a + b;           // Addition: 13
int difference = a - b;    // Subtraction: 7
int product = a * b;       // Multiplication: 30
int quotient = a / b;      // Integer division: 3 (not 3.33!)
int remainder = a % b;     // Modulus (remainder): 1

// Division behavior depends on types
int intDiv = 10 / 3;       // Result: 3 (integer division)
double doubleDiv = 10.0 / 3.0;  // Result: 3.333...

// Increment and decrement
int counter = 5;
counter++;                 // counter is now 6 (postfix increment)
++counter;                 // counter is now 7 (prefix increment)
counter--;                 // counter is now 6 (postfix decrement)
--counter;                 // counter is now 5 (prefix decrement)

// Difference between prefix and postfix
int x = 5;
int y = x++;               // y = 5, x = 6 (x used first, then incremented)
int z = ++x;               // z = 7, x = 7 (x incremented first, then used)
```

A common source of confusion for beginners is integer division. When both operands are integers, the division operator performs integer division, which truncates any decimal portion. To get a decimal result, at least one operand must be a floating-point type. This is why `10 / 3` equals `3`, but `10.0 / 3` equals approximately `3.333`.

### Comparison Operators

Comparison operators compare two values and return a boolean result (`true` or `false`). These operators are fundamental to conditional logic and are used extensively in if statements, loops, and anywhere decisions need to be made based on values.

```csharp
int x = 10;
int y = 20;

bool isEqual = x == y;         // Equal to: false
bool isNotEqual = x != y;      // Not equal to: true
bool isLessThan = x < y;       // Less than: true
bool isGreaterThan = x > y;    // Greater than: false
bool isLessOrEqual = x <= 10;  // Less than or equal: true
bool isGreaterOrEqual = x >= 10;  // Greater than or equal: true

// Comparing strings
string name1 = "Alice";
string name2 = "Alice";
string name3 = "Bob";

bool sameName = name1 == name2;    // true (same content)
bool differentName = name1 == name3;  // false

// String comparison methods for more control
int comparison = string.Compare(name1, name3);  // -1 (name1 comes before name3)
bool equalIgnoreCase = name1.Equals("ALICE", StringComparison.OrdinalIgnoreCase);  // true
```

When comparing strings, the `==` operator compares content by default (unlike some languages where it compares references). However, for case-insensitive comparisons or culture-specific comparisons, use the string comparison methods. For comparing floating-point numbers, be aware that small rounding errors can make exact equality comparisons unreliable—consider checking if the difference is within a small tolerance.

### Logical Operators

Logical operators work with boolean values to combine or modify conditions. They're essential for building complex conditional expressions that check multiple criteria. Understanding operator precedence and short-circuit evaluation is important for writing correct and efficient logical expressions.

```csharp
bool isAdult = true;
bool hasLicense = true;
bool isStudent = false;

// AND operator (&&) - true if both operands are true
bool canDrive = isAdult && hasLicense;  // true
bool adultStudent = isAdult && isStudent;  // false

// OR operator (||) - true if at least one operand is true
bool getsDiscount = isStudent || isAdult;  // true
bool canRentCar = isAdult || hasLicense;  // true

// NOT operator (!) - inverts the boolean value
bool isMinor = !isAdult;  // false
bool isNotStudent = !isStudent;  // true

// Combining multiple conditions
bool eligible = isAdult && (hasLicense || isStudent);
// true && (true || false) = true && true = true

// Short-circuit evaluation
int? value = null;
// bool result = value != null && value > 10;  // Safe - second part not evaluated if first is false
```

The `&&` and `||` operators use short-circuit evaluation: they evaluate the second operand only if necessary. For `&&`, if the first operand is false, the result must be false, so the second operand isn't evaluated. For `||`, if the first operand is true, the result must be true. This behavior is useful for avoiding null reference exceptions and improving performance.

### Assignment Operators

Assignment operators assign values to variables. Beyond the simple assignment operator (`=`), C# provides compound assignment operators that combine an operation with assignment, making code more concise.

```csharp
int score = 100;          // Simple assignment

// Compound assignment operators
score += 10;              // score = score + 10;  (110)
score -= 5;               // score = score - 5;   (105)
score *= 2;               // score = score * 2;   (210)
score /= 3;               // score = score / 3;   (70)
score %= 20;              // score = score % 20;  (10)

// Null-coalescing assignment (C# 8+)
string? name = null;
name ??= "Unknown";       // Assigns "Unknown" only if name is null
Console.WriteLine(name);  // "Unknown"

name ??= "Other";         // Doesn't change - name already has a value
Console.WriteLine(name);  // Still "Unknown"
```

Compound assignment operators are particularly useful in loops for accumulating values, and they make the code's intent clear. The null-coalescing assignment operator (`??=`) is a modern addition that simplifies the common pattern of setting a default value only when a variable is null.

### Operator Precedence

When an expression contains multiple operators, the order in which they're evaluated is determined by operator precedence. Understanding precedence helps you write expressions that produce the expected results. When in doubt, use parentheses to make the order explicit.

```csharp
// Operator precedence (highest to lowest):
// 1. Primary: x.y, f(x), a[i], x++, x--
// 2. Unary: +, -, !, ~, ++x, --x
// 3. Multiplicative: *, /, %
// 4. Additive: +, -
// 5. Relational: <, >, <=, >=
// 6. Equality: ==, !=
// 7. Logical AND: &&
// 8. Logical OR: ||
// 9. Assignment: =, +=, -=, etc.

int result = 2 + 3 * 4;       // 14, not 20 (* has higher precedence than +)
int withParens = (2 + 3) * 4; // 20 (parentheses override precedence)

bool complex = true || false && false;  // true (&& evaluated before ||)
bool withParens2 = (true || false) && false;  // false (parentheses change order)

// Best practice: use parentheses for clarity
bool clear = (isValid && hasPermission) || isAdmin;  // Clear intent
bool confusing = isValid && hasPermission || isAdmin;  // Same result, but unclear
```

While memorizing the complete precedence table isn't necessary, remembering that multiplication has higher precedence than addition, and logical AND has higher precedence than logical OR, covers most common cases. When writing complex expressions, always use parentheses to make your intent explicit, even when not strictly necessary—clarity is more important than brevity.

---

## 7. Control Flow Statements

### The if Statement

The `if` statement is the most fundamental control flow construct. It executes a block of code only if a specified condition is true. This ability to make decisions based on conditions is what allows programs to behave differently under different circumstances, making software dynamic and responsive rather than purely sequential.

```csharp
int temperature = 25;

// Basic if statement
if (temperature > 30)
{
    Console.WriteLine("It's hot outside!");
}

// if-else statement
if (temperature > 30)
{
    Console.WriteLine("It's hot outside!");
}
else
{
    Console.WriteLine("It's not too hot.");
}

// if-else if-else chain
if (temperature > 35)
{
    Console.WriteLine("Extremely hot! Stay indoors.");
}
else if (temperature > 25)
{
    Console.WriteLine("It's warm and pleasant.");
}
else if (temperature > 15)
{
    Console.WriteLine("It's mild. A light jacket might help.");
}
else
{
    Console.WriteLine("It's cold. Bundle up!");
}
```

The condition in an `if` statement must evaluate to a boolean value. This is a key difference from some other languages where non-boolean values can be used as conditions. In C#, you cannot write `if (number)` to check if a number is non-zero—you must explicitly write `if (number != 0)`. This requirement makes code clearer and helps prevent certain types of bugs.

### Nested if Statements

You can place `if` statements inside other `if` statements, creating nested conditions. While this is sometimes necessary, deeply nested conditions can make code hard to read and understand. It's often better to combine conditions using logical operators or restructure the code to reduce nesting.

```csharp
int age = 25;
bool hasLicense = true;

// Nested if statements
if (age >= 18)
{
    if (hasLicense)
    {
        Console.WriteLine("You can drive a car.");
    }
    else
    {
        Console.WriteLine("You need to get a license first.");
    }
}
else
{
    Console.WriteLine("You're too young to drive.");
}

// Equivalent code using logical operators (preferred)
if (age >= 18 && hasLicense)
{
    Console.WriteLine("You can drive a car.");
}
else if (age >= 18 && !hasLicense)
{
    Console.WriteLine("You need to get a license first.");
}
else
{
    Console.WriteLine("You're too young to drive.");
}

// Early return pattern (even cleaner)
if (age < 18)
{
    Console.WriteLine("You're too young to drive.");
    return;  // Or continue/break in loops
}

if (!hasLicense)
{
    Console.WriteLine("You need to get a license first.");
    return;
}

Console.WriteLine("You can drive a car.");
```

### The switch Statement

The `switch` statement provides a cleaner way to handle multiple possible values of a single expression. It's often more readable than a long series of `if-else if` statements when checking a variable against multiple specific values. The switch expression compares the value to each case and executes the matching case's code.

```csharp
int dayOfWeek = 3;
string dayName;

// Traditional switch statement
switch (dayOfWeek)
{
    case 1:
        dayName = "Monday";
        break;
    case 2:
        dayName = "Tuesday";
        break;
    case 3:
        dayName = "Wednesday";
        break;
    case 4:
        dayName = "Thursday";
        break;
    case 5:
        dayName = "Friday";
        break;
    case 6:
    case 7:
        dayName = "Weekend";
        break;
    default:
        dayName = "Invalid day";
        break;
}

Console.WriteLine($"Day: {dayName}");

// Switch statement with patterns (C# 7+)
object obj = "Hello";

switch (obj)
{
    case int i:
        Console.WriteLine($"It's an integer: {i}");
        break;
    case string s:
        Console.WriteLine($"It's a string: {s}");
        break;
    case null:
        Console.WriteLine("It's null");
        break;
    default:
        Console.WriteLine("It's something else");
        break;
}
```

The `break` statement is required at the end of each case block in C#. Unlike C and C++, C# doesn't allow "fall-through" from one case to another (except when cases are grouped with no code between them, as shown in case 6 and 7 above). The `default` case handles any value that doesn't match the other cases and is optional but recommended for handling unexpected values.

### Switch Expressions (C# 8+)

Modern C# introduces switch expressions, which provide a more concise syntax for switch statements that produce a value. Switch expressions are expressions rather than statements, meaning they produce a result that can be assigned to a variable or used in other expressions.

```csharp
int dayOfWeek = 3;

// Switch expression (concise syntax)
string dayName = dayOfWeek switch
{
    1 => "Monday",
    2 => "Tuesday",
    3 => "Wednesday",
    4 => "Thursday",
    5 => "Friday",
    6 or 7 => "Weekend",  // Multiple values with 'or'
    _ => "Invalid day"     // Discard pattern (default)
};

Console.WriteLine(dayName);

// Switch expression with pattern matching
string DescribeNumber(int number) => number switch
{
    < 0 => "Negative",
    0 => "Zero",
    > 0 and < 10 => "Single digit positive",
    >= 10 and < 100 => "Double digit positive",
    >= 100 => "Large positive"
};

Console.WriteLine(DescribeNumber(42));  // "Double digit positive"

// Switch expression with tuples
string GetCategory(int age, bool isStudent) => (age, isStudent) switch
{
    ( < 18, _) => "Minor",
    ( >= 18, true) => "Adult Student",
    ( >= 18, false) => "Adult",
    _ => "Unknown"
};
```

Switch expressions are increasingly preferred in modern C# code for their conciseness and clarity. The arrow syntax (`=>`) separates the pattern from the result, and each case is separated by a comma. The discard pattern (`_`) serves as the default case. The `and` and `or` patterns allow combining conditions in sophisticated ways.

### The Ternary Operator

The conditional operator (`?:`), commonly called the ternary operator, provides a concise way to write simple if-else statements that produce a value. It takes three operands: a condition, a value if true, and a value if false. The ternary operator is ideal for simple conditional assignments but should be avoided for complex logic.

```csharp
int age = 20;

// Traditional if-else
string status1;
if (age >= 18)
{
    status1 = "Adult";
}
else
{
    status1 = "Minor";
}

// Equivalent using ternary operator
string status2 = age >= 18 ? "Adult" : "Minor";

// Ternary in string interpolation
Console.WriteLine($"You are an {(age >= 18 ? "adult" : "minor")}");

// Nested ternary (avoid complex nesting)
int score = 75;
string grade = score >= 90 ? "A" :
               score >= 80 ? "B" :
               score >= 70 ? "C" :
               score >= 60 ? "D" : "F";

// Practical example: handling null
string? name = null;
string displayName = name ?? "Guest";  // Null-coalescing operator
string displayName2 = name != null ? name : "Guest";  // Ternary equivalent
```

While the ternary operator can make simple conditional assignments more concise, overusing it or nesting multiple ternary operators can make code hard to read. As a rule of thumb, if the condition or the values are complex, use a regular if-else statement. The ternary operator shines in simple, self-explanatory cases like the examples above.

---

## 8. Loops and Iteration

### The while Loop

The `while` loop repeatedly executes a block of code as long as a specified condition remains true. The condition is checked before each iteration, so if it's initially false, the loop body never executes. While loops are ideal when you don't know in advance how many iterations you need, but you know the condition that should end the loop.

```csharp
// Basic while loop
int count = 0;
while (count < 5)
{
    Console.WriteLine($"Count: {count}");
    count++;
}
// Output: 0, 1, 2, 3, 4

// While loop for user input validation
string? input;
while (true)
{
    Console.Write("Enter 'quit' to exit: ");
    input = Console.ReadLine();
    
    if (input?.ToLower() == "quit")
    {
        break;  // Exit the loop
    }
    
    Console.WriteLine($"You entered: {input}");
}

// While loop reading until end of file
string? line;
using var reader = new StreamReader("data.txt");
while ((line = reader.ReadLine()) != null)
{
    Console.WriteLine(line);
}

// Warning: infinite loop if condition never becomes false
// while (true)
// {
//     // This runs forever without a break statement
// }
```

A common pattern is using `while (true)` with a `break` statement inside the loop to create a loop that runs until a specific condition is met inside the body. This pattern is useful when the exit condition is complex or when you need to perform setup before checking the condition. Always ensure your while loops have a way to terminate, or they'll run forever (an infinite loop).

### The do-while Loop

The `do-while` loop is similar to the `while` loop, but the condition is checked at the end of each iteration rather than at the beginning. This means the loop body always executes at least once. Do-while loops are useful when you need to perform an action before checking whether to continue.

```csharp
// do-while loop - body executes at least once
int number;
do
{
    Console.Write("Enter a number between 1 and 10: ");
    string? input = Console.ReadLine();
    number = int.TryParse(input, out int result) ? result : 0;
}
while (number < 1 || number > 10);

Console.WriteLine($"You entered: {number}");

// Comparison with while loop
// With while, if condition is initially false, body never runs:
int x = 10;
while (x < 5)  // Condition is false
{
    Console.WriteLine("This never prints");
}

// With do-while, body runs once even if condition is false:
int y = 10;
do
{
    Console.WriteLine("This prints once");  // Runs even though y >= 5
}
while (y < 5);  // Then condition is checked

// Menu system example
int choice;
do
{
    Console.WriteLine("\n--- Menu ---");
    Console.WriteLine("1. Option One");
    Console.WriteLine("2. Option Two");
    Console.WriteLine("3. Exit");
    Console.Write("Select an option: ");
    
    if (int.TryParse(Console.ReadLine(), out choice))
    {
        switch (choice)
        {
            case 1:
                Console.WriteLine("You selected Option One");
                break;
            case 2:
                Console.WriteLine("You selected Option Two");
                break;
            case 3:
                Console.WriteLine("Goodbye!");
                break;
            default:
                Console.WriteLine("Invalid option");
                break;
        }
    }
}
while (choice != 3);
```

The do-while loop is particularly useful for input validation, where you always want to prompt the user at least once, and for menu-driven programs where the menu should always be displayed before checking if the user wants to exit.

### The for Loop

The `for` loop is designed for situations where you know (or can calculate) how many times you need to iterate. It combines initialization, condition checking, and iteration in a single line, making the loop's purpose clear at a glance. For loops are the most common type of loop when working with arrays and other indexed collections.

```csharp
// Basic for loop structure
// for (initialization; condition; iteration)
for (int i = 0; i < 5; i++)
{
    Console.WriteLine($"Iteration: {i}");
}
// Output: 0, 1, 2, 3, 4

// Counting backwards
for (int i = 10; i >= 0; i--)
{
    Console.WriteLine($"Countdown: {i}");
}

// Stepping by different amounts
for (int i = 0; i <= 20; i += 5)
{
    Console.WriteLine(i);  // 0, 5, 10, 15, 20
}

// Nested for loops (e.g., for 2D grids)
for (int row = 0; row < 3; row++)
{
    for (int col = 0; col < 3; col++)
    {
        Console.Write($"({row},{col}) ");
    }
    Console.WriteLine();
}
// Output:
// (0,0) (0,1) (0,2)
// (1,0) (1,1) (1,2)
// (2,0) (2,1) (2,2)

// Multiple variables in for loop
for (int i = 0, j = 10; i < j; i++, j--)
{
    Console.WriteLine($"i={i}, j={j}");
}
```

The for loop consists of three parts separated by semicolons: the initialization (runs once before the loop), the condition (checked before each iteration), and the iterator (runs after each iteration). All three parts are optional—an empty condition creates an infinite loop. Variables declared in the initialization section are scoped to the loop and cannot be accessed outside it.

### The foreach Loop

The `foreach` loop iterates over each element in a collection, such as an array, list, or any type that implements `IEnumerable`. Unlike the for loop, `foreach` doesn't use an index variable—it directly provides each element in sequence. This makes the code cleaner and eliminates off-by-one errors common with indexed loops.

```csharp
// foreach with arrays
string[] fruits = { "Apple", "Banana", "Cherry", "Date" };
foreach (string fruit in fruits)
{
    Console.WriteLine(fruit);
}

// foreach with numbers
int[] numbers = { 1, 2, 3, 4, 5 };
int sum = 0;
foreach (int num in numbers)
{
    sum += num;
}
Console.WriteLine($"Sum: {sum}");  // Output: Sum: 15

// foreach with strings (iterates over characters)
string message = "Hello";
foreach (char c in message)
{
    Console.WriteLine(c);
}
// Output: H, e, l, l, o (each on new line)

// Cannot modify collection during foreach
var list = new List<int> { 1, 2, 3, 4, 5 };
foreach (int num in list)
{
    // list.Remove(num);  // Exception! Can't modify during iteration
    Console.WriteLine(num);
}

// To modify, use for loop or iterate over a copy
for (int i = list.Count - 1; i >= 0; i--)
{
    if (list[i] % 2 == 0)
    {
        list.RemoveAt(i);  // Safe with backwards iteration
    }
}
```

The `foreach` loop is read-only for value types—you cannot modify the elements through the loop variable. For reference types, you can modify the object's properties, but you can't replace the object in the collection. Also, you cannot add or remove items from the collection while iterating over it with `foreach`; doing so throws an `InvalidOperationException`.

### Break and Continue

The `break` and `continue` statements provide additional control over loop execution. `break` immediately exits the loop entirely, while `continue` skips the rest of the current iteration and proceeds to the next iteration. These statements help handle edge cases and can make loop logic clearer by avoiding deeply nested conditions.

```csharp
// break - exit loop entirely
for (int i = 0; i < 10; i++)
{
    if (i == 5)
    {
        Console.WriteLine("Breaking at 5");
        break;  // Exit loop completely
    }
    Console.WriteLine(i);
}
// Output: 0, 1, 2, 3, 4, "Breaking at 5"

// continue - skip to next iteration
for (int i = 0; i < 10; i++)
{
    if (i % 2 == 0)
    {
        continue;  // Skip even numbers
    }
    Console.WriteLine(i);  // Only prints odd numbers
}
// Output: 1, 3, 5, 7, 9

// Practical example: searching
string[] names = { "Alice", "Bob", "Charlie", "David", "Eve" };
string searchFor = "Charlie";
bool found = false;

foreach (string name in names)
{
    if (name == searchFor)
    {
        Console.WriteLine($"Found {searchFor}!");
        found = true;
        break;  // No need to continue searching
    }
}

if (!found)
{
    Console.WriteLine($"{searchFor} not found");
}

// Break in nested loops
for (int i = 0; i < 3; i++)
{
    for (int j = 0; j < 3; j++)
    {
        if (i == 1 && j == 1)
        {
            break;  // Only breaks inner loop
        }
        Console.WriteLine($"({i},{j})");
    }
}
```

Note that `break` only exits the innermost loop. If you need to exit from a nested loop, you can use a flag variable, a labeled break (not available in C#), or refactor the code into a method and use `return`. The `continue` statement in a `for` loop jumps to the iterator expression, while in a `while` or `do-while` loop, it jumps to the condition check.

---

## 9. Arrays

### What is an Array?

An array is a fixed-size collection of elements of the same type stored in contiguous memory locations. Arrays are among the most fundamental data structures in programming, providing a way to store and access multiple values using a single variable name with an index. The index starts at 0 for the first element and goes up to one less than the array's length. Understanding arrays is essential because many other collection types build upon array concepts.

Arrays in C# are reference types, meaning an array variable stores a reference to the actual data stored on the heap. Once an array is created, its size cannot be changed—if you need a dynamically sized collection, you would use a `List<T>` instead. Arrays are zero-indexed, meaning the first element is at index 0, and the last element is at index `Length - 1`.

### Creating and Initializing Arrays

There are several ways to create arrays in C#, offering flexibility depending on your needs. You can declare an array variable, create the array with a specific size, and populate it later, or you can create and initialize an array in a single statement.

```csharp
// Declare and create array with specific size
int[] numbers = new int[5];  // Array of 5 integers, initialized to 0

// Declare, create, and initialize in one statement
int[] scores = new int[] { 95, 87, 92, 88, 91 };

// Simplified syntax (type inferred)
int[] ages = { 25, 30, 35, 40, 45 };

// String array
string[] names = { "Alice", "Bob", "Charlie" };

// Array of objects
object[] mixed = { 1, "Hello", 3.14, true };

// Create array with default values
int[] zeros = new int[5];           // All zeros: { 0, 0, 0, 0, 0 }
string[] empty = new string[3];     // All nulls: { null, null, null }
bool[] flags = new bool[4];         // All false: { false, false, false, false }

// Create array with repeated values (C# 12+)
int[] repeated = new int[5];        // Still need to populate manually
// Or use Enumerable
int[] allTwos = Enumerable.Repeat(2, 5).ToArray();
```

When you create an array with the `new` keyword and a size, each element is initialized to its default value: 0 for numeric types, false for boolean, and null for reference types. The simplified syntax without `new` can only be used when declaring and initializing in the same statement.

### Accessing Array Elements

Array elements are accessed using square brackets with an index. You can both read from and write to array elements using this syntax. Attempting to access an index outside the valid range (less than 0 or greater than or equal to the array's length) throws an `IndexOutOfRangeException`.

```csharp
int[] numbers = { 10, 20, 30, 40, 50 };

// Reading elements
int first = numbers[0];     // 10 (first element)
int third = numbers[2];     // 30 (third element)
int last = numbers[4];      // 50 (last element)

// Writing elements
numbers[0] = 15;            // Array is now { 15, 20, 30, 40, 50 }
numbers[2] = numbers[1] + numbers[3];  // numbers[2] = 60

// Accessing last element using Length
int lastIndex = numbers.Length - 1;
int lastElement = numbers[lastIndex];

// Common pattern: iterate through array with for loop
for (int i = 0; i < numbers.Length; i++)
{
    Console.WriteLine($"numbers[{i}] = {numbers[i]}");
}

// Using foreach (read-only access)
foreach (int num in numbers)
{
    Console.WriteLine(num);
}

// Index from end operator (C# 8+)
int lastItem = numbers[^1];    // Last element
int secondLast = numbers[^2];  // Second to last element
```

Modern C# (8.0 and later) introduces the index-from-end operator (`^`), which allows you to access elements counting from the end of the array. `^1` refers to the last element, `^2` to the second-to-last, and so on. This is particularly useful when you need to access elements relative to the end without calculating the index manually.

### Multi-Dimensional Arrays

C# supports two types of multi-dimensional arrays: rectangular arrays (true multi-dimensional) and jagged arrays (arrays of arrays). Rectangular arrays have a fixed number of dimensions, with each dimension's size specified when the array is created. Jagged arrays are arrays where each element is itself an array, potentially of different lengths.

```csharp
// Rectangular (2D) array - single memory block
int[,] matrix = new int[3, 4];  // 3 rows, 4 columns

// Initialize 2D array
int[,] grid = {
    { 1, 2, 3 },
    { 4, 5, 6 },
    { 7, 8, 9 }
};

// Access 2D array elements
int center = grid[1, 1];  // 5 (row 1, column 1)

// Iterate through 2D array
for (int row = 0; row < grid.GetLength(0); row++)
{
    for (int col = 0; col < grid.GetLength(1); col++)
    {
        Console.Write($"{grid[row, col]} ");
    }
    Console.WriteLine();
}

// Get dimensions
int rows = grid.GetLength(0);   // Number of rows
int cols = grid.GetLength(1);   // Number of columns
int total = grid.Length;        // Total elements (9)

// Jagged array - array of arrays
int[][] jagged = new int[3][];
jagged[0] = new int[] { 1, 2, 3 };
jagged[1] = new int[] { 4, 5 };
jagged[2] = new int[] { 6, 7, 8, 9 };

// Access jagged array
int value = jagged[0][2];  // 3 (first array, third element)

// Iterate through jagged array
for (int i = 0; i < jagged.Length; i++)
{
    for (int j = 0; j < jagged[i].Length; j++)
    {
        Console.Write($"{jagged[i][j]} ");
    }
    Console.WriteLine();
}
```

Rectangular arrays are useful for representing grids, matrices, or any data with a fixed structure. Jagged arrays are more memory-efficient when rows have different lengths and are also more flexible, as each row can be resized independently.

### Array Methods and Properties

The `Array` class provides numerous methods for working with arrays, including sorting, searching, and manipulating elements. These methods are static methods called on the `Array` class, while properties like `Length` are instance members accessed on the array object itself.

```csharp
int[] numbers = { 5, 2, 8, 1, 9, 3, 7, 4, 6 };

// Properties
int length = numbers.Length;     // 9

// Sorting
Array.Sort(numbers);             // { 1, 2, 3, 4, 5, 6, 7, 8, 9 }
Array.Reverse(numbers);          // { 9, 8, 7, 6, 5, 4, 3, 2, 1 }

// Searching
int index = Array.IndexOf(numbers, 5);    // Index of value 5
int notFound = Array.IndexOf(numbers, 99); // -1 if not found
bool contains = Array.BinarySearch(numbers, 5) >= 0;  // Requires sorted array

// Copying
int[] copy = new int[numbers.Length];
Array.Copy(numbers, copy, numbers.Length);

// Or use Clone (returns object, needs casting)
int[] cloned = (int[])numbers.Clone();

// Resizing (creates new array)
Array.Resize(ref numbers, 15);   // Creates new array with new size

// Clearing elements
Array.Clear(numbers, 0, 3);      // Sets first 3 elements to default

// Finding elements
int[] moreNumbers = { 1, 5, 10, 15, 20, 25 };
int firstOverTen = Array.Find(moreNumbers, n => n > 10);  // 15
int[] allOverTen = Array.FindAll(moreNumbers, n => n > 10);  // { 15, 20, 25 }
bool anyOverTwenty = Array.Exists(moreNumbers, n => n > 20);  // true
```

The `Array.Find` and related methods use predicates (lambda expressions) to define search conditions. These methods are more flexible than simple `IndexOf` searches because they can match based on any criteria. We'll cover lambda expressions in more detail in the advanced topics.

---

## 10. Methods (Functions)

### What are Methods?

A method is a reusable block of code that performs a specific task. Methods are fundamental to organizing code—they allow you to break complex problems into smaller, manageable pieces, avoid code duplication, and create code that's easier to understand, test, and maintain. When you find yourself writing the same code multiple times, that's a sign you should extract it into a method.

Methods in C# have a clear structure: they can accept input through parameters, perform operations, and optionally return a value to the caller. A method's signature includes its name, return type, and parameter list. Understanding how to define and use methods effectively is one of the most important skills in programming.

### Defining and Calling Methods

Methods are defined with a return type, a name, optional parameters, and a body containing the code to execute. The return type specifies what kind of value the method produces, or `void` if it produces no value. Parameters define the inputs the method expects.

```csharp
// Method with no parameters and no return value (void)
void SayHello()
{
    Console.WriteLine("Hello, World!");
}

// Calling the method
SayHello();  // Output: Hello, World!

// Method with parameters and no return value
void Greet(string name)
{
    Console.WriteLine($"Hello, {name}!");
}

Greet("Alice");  // Output: Hello, Alice!
Greet("Bob");    // Output: Hello, Bob!

// Method with parameters and return value
int Add(int a, int b)
{
    return a + b;
}

int sum = Add(5, 3);  // sum = 8
Console.WriteLine(sum);

// Method with early return
bool IsPositive(int number)
{
    if (number > 0)
    {
        return true;
    }
    return false;
}

// Simplified version
bool IsPositiveSimple(int number) => number > 0;
```

The `return` statement immediately exits the method and sends the specified value back to the caller. For `void` methods, you can use `return;` without a value to exit early, or simply let execution reach the end of the method. Methods should generally have a single responsibility—do one thing well—making them easier to name, test, and reuse.

### Parameters and Arguments

Parameters are variables defined in a method's signature that receive values when the method is called. The values passed to parameters are called arguments. C# provides several parameter modifiers that change how arguments are passed to methods, giving you flexibility in how methods interact with caller data.

```csharp
// Value parameters (default) - copy of the argument is passed
void IncrementValue(int x)
{
    x++;  // Only modifies the local copy
}

int number = 5;
IncrementValue(number);
Console.WriteLine(number);  // Still 5 (unchanged)

// ref parameter - reference to original variable is passed
void IncrementRef(ref int x)
{
    x++;  // Modifies the original variable
}

int num = 5;
IncrementRef(ref num);
Console.WriteLine(num);  // 6 (changed!)

// out parameter - method must assign a value
bool TryParseInt(string input, out int result)
{
    return int.TryParse(input, out result);
}

if (TryParseInt("42", out int parsed))
{
    Console.WriteLine($"Parsed: {parsed}");
}

// in parameter - read-only reference (C# 7.2+)
void DisplayValue(in int x)
{
    // x = 10;  // Error: cannot modify
    Console.WriteLine(x);
}

// params parameter - accepts variable number of arguments
int Sum(params int[] numbers)
{
    int total = 0;
    foreach (int n in numbers)
    {
        total += n;
    }
    return total;
}

int total1 = Sum(1, 2, 3);           // 6
int total2 = Sum(1, 2, 3, 4, 5);     // 15
int total3 = Sum(new int[] { 1, 2 }); // 3
```

The `ref` keyword requires that the variable be initialized before being passed, and allows the method to modify it. The `out` keyword doesn't require initialization before passing, but the method must assign a value before returning. The `params` keyword allows a method to accept any number of arguments of the specified type, which are collected into an array.

### Method Overloading

Method overloading allows you to define multiple methods with the same name but different parameter lists. This is useful when you want to provide different ways to call a method with different types or numbers of parameters. The compiler determines which overload to call based on the arguments provided.

```csharp
// Overloaded methods
int Add(int a, int b)
{
    return a + b;
}

double Add(double a, double b)
{
    return a + b;
}

int Add(int a, int b, int c)
{
    return a + b + c;
}

// Calling overloaded methods
int sum1 = Add(1, 2);           // Calls first overload
double sum2 = Add(1.5, 2.5);     // Calls second overload
int sum3 = Add(1, 2, 3);         // Calls third overload

// Overloading with optional parameters (C# 4+)
void PrintMessage(string message, bool uppercase = false, int repeat = 1)
{
    for (int i = 0; i < repeat; i++)
    {
        Console.WriteLine(uppercase ? message.ToUpper() : message);
    }
}

PrintMessage("Hello");                    // Hello
PrintMessage("Hello", true);              // HELLO
PrintMessage("Hello", false, 3);          // Hello (3 times)
PrintMessage("Hello", repeat: 3);         // Hello (3 times) - named argument
```

When using optional parameters, all optional parameters must come after required parameters in the parameter list. Named arguments allow you to specify arguments by name rather than position, which is particularly useful with optional parameters when you want to skip some optional parameters.

### Expression-Bodied Methods

For simple methods that consist of a single expression, C# provides expression-bodied member syntax, which is more concise than the traditional block syntax. This is particularly useful for small utility methods and property getters.

```csharp
// Traditional method
int Square(int x)
{
    return x * x;
}

// Expression-bodied method (equivalent)
int Square(int x) => x * x;

// More examples
bool IsEven(int n) => n % 2 == 0;
string GetGreeting(string name) => $"Hello, {name}!";
void Log(string message) => Console.WriteLine($"[{DateTime.Now}] {message}");

// Useful for mathematical operations
double CalculateCircleArea(double radius) => Math.PI * radius * radius;
double CelsiusToFahrenheit(double celsius) => celsius * 9 / 5 + 32;
```

Expression-bodied methods make code more concise and often more readable when the method's purpose is a simple calculation or transformation. However, if a method needs multiple statements, loops, or complex logic, use the traditional block syntax with curly braces.

---

## 11. String Manipulation

### String Basics

Strings in C# are immutable sequences of Unicode characters. Once a string is created, its contents cannot be changed—any operation that appears to modify a string actually creates a new string. This immutability has important implications for performance and memory usage, particularly when building strings through repeated concatenation.

```csharp
// String creation
string greeting = "Hello";
string empty = "";
string alsoEmpty = string.Empty;
string multiLine = """
    Line 1
    Line 2
    Line 3
    """;

// String properties
int length = greeting.Length;     // 5
char firstChar = greeting[0];     // 'H'
char lastChar = greeting[^1];     // 'o'

// Strings are immutable
string original = "Hello";
string modified = original.ToUpper();
Console.WriteLine(original);   // "Hello" (unchanged)
Console.WriteLine(modified);   // "HELLO" (new string)

// Character access
for (int i = 0; i < greeting.Length; i++)
{
    Console.WriteLine($"greeting[{i}] = '{greeting[i]}'");
}
```

Because strings are immutable, operations that might seem to modify a string, like `ToUpper()`, `ToLower()`, or `Trim()`, actually return new strings. The original string remains unchanged. This is important to remember when chaining string operations or when performance is critical.

### String Concatenation and Interpolation

C# provides several ways to combine strings. String interpolation is the modern, preferred approach for most scenarios because it's readable and efficient. For building strings through repeated concatenation in loops, `StringBuilder` is more efficient.

```csharp
// String concatenation with +
string firstName = "John";
string lastName = "Doe";
string fullName = firstName + " " + lastName;  // "John Doe"

// String concatenation with String.Concat
string concatenated = string.Concat("Hello", " ", "World");  // "Hello World"

// String interpolation (preferred)
int age = 30;
string info = $"{firstName} {lastName} is {age} years old.";
Console.WriteLine(info);  // "John Doe is 30 years old."

// Interpolation with format specifiers
double price = 19.99;
int quantity = 5;
string receipt = $"Total: {price * quantity:C}";  // "Total: $99.95"
string percentage = $"Discount: {0.15:P0}";        // "Discount: 15%"
string formatted = $"Date: {DateTime.Now:yyyy-MM-dd}";  // "Date: 2024-01-15"

// Verbatim strings for paths and multi-line text
string path = @"C:\Users\John\Documents\file.txt";
string query = @"
    SELECT *
    FROM Users
    WHERE Active = 1
";

// Raw string literals (C# 11+)
string json = """
    {
        "name": "John",
        "age": 30
    }
    """;
```

String interpolation expressions can include any valid C# expression, including method calls, mathematical operations, and conditional expressions. Format specifiers follow a colon after the expression and control how the value is formatted. Common specifiers include `C` for currency, `P` for percentage, `D` for decimal integers, and `F` for fixed-point numbers.

### Common String Methods

The `string` class provides numerous methods for manipulating and analyzing strings. These methods don't modify the original string—they return new strings or other values based on the operation.

```csharp
string text = "  Hello, World!  ";

// Trimming
string trimmed = text.Trim();           // "Hello, World!"
string trimStart = text.TrimStart();    // "Hello, World!  "
string trimEnd = text.TrimEnd();        // "  Hello, World!"

// Case conversion
string upper = text.ToUpper();          // "  HELLO, WORLD!  "
string lower = text.ToLower();          // "  hello, world!  "

// Substring
string hello = trimmed.Substring(0, 5);  // "Hello"
string world = trimmed.Substring(7);     // "World!"

// Replacing
string replaced = text.Replace("World", "C#");  // "  Hello, C#!  "

// Contains, StartsWith, EndsWith
bool containsHello = text.Contains("Hello");     // true
bool startsWith = trimmed.StartsWith("Hello");   // true
bool endsWith = trimmed.EndsWith("!");           // true

// Index finding
int commaIndex = text.IndexOf(',');         // 7
int worldIndex = text.IndexOf("World");     // 9
int lastIndex = text.LastIndexOf('l');      // 10

// Splitting
string csv = "apple,banana,cherry,date";
string[] fruits = csv.Split(',');  // ["apple", "banana", "cherry", "date"]

string sentence = "Hello World from C#";
string[] words = sentence.Split(' ');  // ["Hello", "World", "from", "C#"]

// Joining
string joined = string.Join(" - ", fruits);  // "apple - banana - cherry - date"

// Padding
string padded = "Hello".PadLeft(10, '*');   // "*****Hello"
string paddedRight = "Hello".PadRight(10);  // "Hello     "
```

These methods cover most common string manipulation needs. Remember that string methods don't modify the original string—they always return a new string. If you need to build a string through many operations, consider using `StringBuilder` for better performance.

### StringBuilder for Efficient String Building

When you need to build a string through many concatenations (especially in loops), using `StringBuilder` is significantly more efficient than using string concatenation. `StringBuilder` maintains an internal buffer that it modifies in place, avoiding the creation of many intermediate string objects.

```csharp
using System.Text;

// Inefficient approach - creates many intermediate strings
string result = "";
for (int i = 0; i < 1000; i++)
{
    result += i + " ";  // Creates a new string each iteration
}

// Efficient approach with StringBuilder
var sb = new StringBuilder();
for (int i = 0; i < 1000; i++)
{
    sb.Append(i);
    sb.Append(' ');
}
string efficient = sb.ToString();

// StringBuilder methods
var builder = new StringBuilder();

builder.Append("Hello");           // Append string
builder.Append(' ');               // Append character
builder.AppendLine("World");       // Append with newline
builder.AppendFormat("Today is {0}", DateTime.Now.ToShortDateString());

builder.Insert(6, "Beautiful ");   // Insert at position
builder.Remove(0, 6);              // Remove characters
builder.Replace("World", "C#");    // Replace text

string final = builder.ToString();

// StringBuilder with initial capacity
var largeBuilder = new StringBuilder(10000);  // Pre-allocate buffer
```

Use `StringBuilder` when you're building strings through many operations, especially in loops or when the final size is unknown. For simple concatenation or a small number of operations, regular string operations are fine and often more readable.

### String Comparison

Comparing strings correctly is important for both correctness and performance. C# provides multiple ways to compare strings, with options for case sensitivity and culture-specific rules.

```csharp
// Equality operators (ordinal comparison)
string a = "Hello";
string b = "Hello";
bool areEqual = a == b;                    // true

// Case-sensitive comparison
string c = "hello";
bool equalCaseSensitive = string.Equals(a, c);                           // false
bool equalCaseInsensitive = string.Equals(a, c, StringComparison.OrdinalIgnoreCase);  // true

// Compare method returns -1, 0, or 1
int comparison = string.Compare("apple", "banana");  // -1 (apple comes before banana)
int sameResult = string.Compare("apple", "apple");   // 0 (equal)
int reverseResult = string.Compare("banana", "apple");  // 1 (banana comes after)

// CompareTo instance method
int result = "apple".CompareTo("banana");  // -1

// Best practices for comparison
// Use Ordinal for exact byte matching (fastest, most predictable)
bool exactMatch = string.Equals(a, c, StringComparison.Ordinal);  // false

// Use OrdinalIgnoreCase for case-insensitive comparison
bool ignoreCase = string.Equals(a, c, StringComparison.OrdinalIgnoreCase);  // true

// For user-facing comparisons, consider culture
var culture = new System.Globalization.CultureInfo("en-US");
bool cultureCompare = string.Equals("resume", "RESUME", 
    StringComparison.CurrentCultureIgnoreCase);

// Checking for empty or null strings
string? input = null;
bool isNullOrEmpty = string.IsNullOrEmpty(input);      // true
bool isNullOrWhiteSpace = string.IsNullOrWhiteSpace("   ");  // true
```

For most programmatic comparisons, use `StringComparison.Ordinal` or `StringComparison.OrdinalIgnoreCase`. The `CurrentCulture` comparisons are appropriate for user-facing comparisons where cultural sorting rules matter, but they're slower and can behave differently on different systems.

---

## 12. Exception Handling Basics

### What are Exceptions?

Exceptions are runtime errors that disrupt the normal flow of program execution. When an exceptional situation occurs (like dividing by zero, accessing a null reference, or reading a non-existent file), the runtime "throws" an exception. If this exception isn't handled, the program crashes. Exception handling allows you to anticipate and respond to errors gracefully.

C# uses a structured exception handling mechanism with `try`, `catch`, and `finally` blocks. Code that might fail is placed in a `try` block, code to handle specific exceptions goes in `catch` blocks, and code that should run regardless of success or failure goes in a `finally` block. This structure provides a clear way to separate error-prone code from error-handling code.

### Try-Catch Blocks

The basic exception handling pattern wraps potentially failing code in a `try` block, followed by one or more `catch` blocks that handle specific exception types.

```csharp
// Basic try-catch
try
{
    Console.Write("Enter a number: ");
    string? input = Console.ReadLine();
    int number = int.Parse(input!);
    Console.WriteLine($"You entered: {number}");
}
catch (FormatException)
{
    Console.WriteLine("Invalid input. Please enter a valid number.");
}

// Catching specific exceptions
try
{
    int[] numbers = { 1, 2, 3 };
    Console.Write("Enter an index: ");
    int index = int.Parse(Console.ReadLine()!);
    Console.WriteLine($"Value: {numbers[index]}");
}
catch (FormatException)
{
    Console.WriteLine("Please enter a valid number.");
}
catch (IndexOutOfRangeException)
{
    Console.WriteLine("Index out of range. Please enter 0, 1, or 2.");
}

// Catching with exception variable
try
{
    int result = 10 / int.Parse(Console.ReadLine()!);
    Console.WriteLine($"Result: {result}");
}
catch (DivideByZeroException ex)
{
    Console.WriteLine($"Error: {ex.Message}");
}
catch (Exception ex)  // Catch-all for any exception
{
    Console.WriteLine($"Unexpected error: {ex.GetType().Name} - {ex.Message}");
}
```

Always catch specific exception types before more general types. The catch blocks are evaluated in order, and the first matching catch block is executed. A catch block without a type catches all exceptions, which should generally be avoided except at the top level of an application where you want to prevent crashes.

### The Finally Block

The `finally` block contains code that executes whether or not an exception occurred. This is essential for cleanup operations like closing files, releasing resources, or closing database connections. The finally block always executes, even if an exception is thrown or a return statement is encountered.

```csharp
// try-catch-finally
StreamReader? reader = null;
try
{
    reader = new StreamReader("data.txt");
    string? line;
    while ((line = reader.ReadLine()) != null)
    {
        Console.WriteLine(line);
    }
}
catch (FileNotFoundException)
{
    Console.WriteLine("File not found.");
}
catch (IOException ex)
{
    Console.WriteLine($"Error reading file: {ex.Message}");
}
finally
{
    // This always executes
    reader?.Dispose();
    Console.WriteLine("Cleanup complete.");
}

// Using statement (preferred for IDisposable objects)
// Automatically calls Dispose in finally block
try
{
    using var fileReader = new StreamReader("data.txt");
    string? line;
    while ((line = fileReader.ReadLine()) != null)
    {
        Console.WriteLine(line);
    }
}
catch (FileNotFoundException)
{
    Console.WriteLine("File not found.");
}
// Dispose is called automatically when exiting the using block
```

The `using` statement is syntactic sugar for a try-finally pattern that calls `Dispose()` on objects implementing `IDisposable`. For resource management, prefer `using` statements over manual try-finally blocks because they're cleaner and less error-prone.

### Throwing Exceptions

You can throw exceptions to indicate error conditions in your own code. When throwing exceptions, provide meaningful messages that help diagnose the problem. You can throw new exceptions or rethrow caught exceptions to propagate them up the call stack.

```csharp
// Throwing exceptions
int Divide(int numerator, int denominator)
{
    if (denominator == 0)
    {
        throw new DivideByZeroException("Cannot divide by zero.");
    }
    return numerator / denominator;
}

// Validating and throwing
void SetAge(int age)
{
    if (age < 0)
    {
        throw new ArgumentOutOfRangeException(nameof(age), "Age cannot be negative.");
    }
    if (age > 150)
    {
        throw new ArgumentOutOfRangeException(nameof(age), "Age seems unreasonable.");
    }
    // Set age...
}

// Rethrowing exceptions
try
{
    // Some operation
}
catch (Exception ex)
{
    // Log the exception
    Console.WriteLine($"Logging error: {ex.Message}");
    
    // Rethrow - preserves original stack trace
    throw;
}

// Wrapping exceptions
try
{
    // Some operation
}
catch (Exception ex)
{
    throw new InvalidOperationException("Operation failed", ex);
}
```

When throwing exceptions, choose appropriate exception types that accurately describe the error condition. Common exception types include `ArgumentException`, `ArgumentNullException`, `ArgumentOutOfRangeException`, `InvalidOperationException`, `NotSupportedException`, and `InvalidOperationException`. For application-specific errors, you can create custom exception classes.

### Common Exception Types

Understanding common exception types helps you write appropriate error handling and debug issues more effectively.

```csharp
// NullReferenceException - accessing null reference
string? s = null;
// int length = s.Length;  // NullReferenceException

// ArgumentNullException - null passed where not expected
void Process(string data)
{
    if (data == null)
        throw new ArgumentNullException(nameof(data));
    // Process data...
}

// ArgumentOutOfRangeException - value outside valid range
int[] array = new int[5];
// int item = array[10];  // IndexOutOfRangeException

// FormatException - invalid format for parsing
// int.Parse("abc");  // FormatException

// OverflowException - arithmetic overflow
checked
{
    // int big = int.MaxValue + 1;  // OverflowException
}

// InvalidOperationException - object in invalid state
// enumerator.MoveNext();  // If collection modified

// FileNotFoundException, IOException - file operations
// DirectoryNotFoundException - directory doesn't exist

// DivideByZeroException - integer division by zero
// int x = 10 / 0;  // DivideByZeroException
```

---

## 13. Console Input and Output

### Basic Console Output

The `Console` class provides methods for interacting with the console window, including outputting text and reading input. While modern applications typically use graphical user interfaces, console I/O remains fundamental for learning, debugging, and building command-line tools.

```csharp
// Basic output
Console.Write("Hello ");       // No newline
Console.Write("World");
Console.WriteLine();           // Just a newline
Console.WriteLine("Hello, World!");  // Text with newline

// Formatted output
string name = "Alice";
int age = 30;
Console.WriteLine("Name: " + name + ", Age: " + age);
Console.WriteLine("Name: {0}, Age: {1}", name, age);  // Composite formatting
Console.WriteLine($"Name: {name}, Age: {age}");  // String interpolation (preferred)

// Formatting numbers
double price = 19.99;
int count = 42;
Console.WriteLine($"Price: {price:C}");       // Currency: $19.99
Console.WriteLine($"Count: {count:D5}");       // Decimal with padding: 00042
Console.WriteLine($"Percent: {0.5:P0}");       // Percentage: 50%

// Formatting dates
DateTime now = DateTime.Now;
Console.WriteLine($"Date: {now:d}");           // Short date
Console.WriteLine($"Time: {now:T}");           // Long time
Console.WriteLine($"Full: {now:F}");           // Full date/time
Console.WriteLine($"Custom: {now:yyyy-MM-dd HH:mm:ss}");

// Escape sequences
Console.WriteLine("Line 1\nLine 2");           // Newline
Console.WriteLine("Column 1\tColumn 2");       // Tab
Console.WriteLine("Path: C:\\Users\\John");    // Escaped backslash
Console.WriteLine("Quote: \"Hello\"");         // Escaped quote
```

### Reading Console Input

Reading input from the console allows programs to interact with users. The `Console.ReadLine()` method reads a line of text until the user presses Enter. For other data types, you need to parse the input string.

```csharp
// Basic string input
Console.Write("Enter your name: ");
string? name = Console.ReadLine();
Console.WriteLine($"Hello, {name}!");

// Reading numbers with validation
Console.Write("Enter your age: ");
string? ageInput = Console.ReadLine();
if (int.TryParse(ageInput, out int age))
{
    Console.WriteLine($"You are {age} years old.");
}
else
{
    Console.WriteLine("Invalid age entered.");
}

// Reading with null checking
Console.Write("Enter something: ");
string? input = Console.ReadLine();
if (string.IsNullOrEmpty(input))
{
    Console.WriteLine("You didn't enter anything.");
}
else
{
    Console.WriteLine($"You entered: {input}");
}

// Reading a single character
Console.Write("Press any key to continue...");
ConsoleKeyInfo key = Console.ReadKey();
Console.WriteLine($"\nYou pressed: {key.KeyChar}");

// Reading without echo (for passwords)
Console.Write("Enter password: ");
string password = "";
ConsoleKeyInfo keyInfo;
do
{
    keyInfo = Console.ReadKey(true);
    if (keyInfo.Key != ConsoleKey.Enter)
    {
        password += keyInfo.KeyChar;
        Console.Write("*");
    }
}
while (keyInfo.Key != ConsoleKey.Enter);
Console.WriteLine($"\nPassword length: {password.Length}");
```

### Console Color and Formatting

The console supports changing text and background colors, which can improve the user experience for command-line applications.

```csharp
// Text colors
Console.ForegroundColor = ConsoleColor.Green;
Console.WriteLine("Success message in green");

Console.ForegroundColor = ConsoleColor.Red;
Console.WriteLine("Error message in red");

Console.ForegroundColor = ConsoleColor.Yellow;
Console.WriteLine("Warning message in yellow");

// Reset to default
Console.ResetColor();

// Background colors
Console.BackgroundColor = ConsoleColor.Blue;
Console.ForegroundColor = ConsoleColor.White;
Console.WriteLine("White text on blue background");
Console.ResetColor();

// Creating a simple menu
void DisplayMenu()
{
    Console.Clear();
    Console.WriteLine("=== MAIN MENU ===");
    Console.WriteLine("1. Option One");
    Console.WriteLine("2. Option Two");
    Console.WriteLine("3. Option Three");
    Console.WriteLine("Q. Quit");
    Console.WriteLine("=================");
    Console.Write("Select an option: ");
}

// Console position
Console.SetCursorPosition(10, 5);
Console.Write("Text at position (10, 5)");

// Get console dimensions
int width = Console.WindowWidth;
int height = Console.WindowHeight;
Console.WriteLine($"Console size: {width} x {height}");
```

---

## 14. Collections: List and Dictionary

### Introduction to Collections

While arrays have a fixed size, real-world applications often need collections that can grow and shrink dynamically. C# provides a rich set of collection types in the `System.Collections.Generic` namespace. The most commonly used are `List<T>` for ordered collections and `Dictionary<TKey, TValue>` for key-value pairs.

### Working with List<T>

`List<T>` is a dynamic array that can grow or shrink in size. It provides methods for adding, removing, inserting, and searching for elements. The `<T>` syntax indicates a generic type—you specify what type of elements the list will contain.

```csharp
using System.Collections.Generic;

// Creating lists
List<int> numbers = new List<int>();
List<string> names = new List<string>();
var scores = new List<double>();  // Type inferred

// Adding elements
numbers.Add(1);
numbers.Add(2);
numbers.Add(3);

names.Add("Alice");
names.Add("Bob");

// Adding multiple elements
numbers.AddRange(new int[] { 4, 5, 6 });
numbers.AddRange(new List<int> { 7, 8, 9 });

// Initialize with values
List<string> colors = new List<string> { "Red", "Green", "Blue" };

// Accessing elements
int firstNumber = numbers[0];       // First element
string secondColor = colors[1];     // "Green"

// Properties
int count = numbers.Count;          // Number of elements
int capacity = numbers.Capacity;    // Internal array size

// Modifying elements
numbers[0] = 100;                   // Change first element

// Removing elements
numbers.Remove(3);                  // Remove first occurrence of 3
numbers.RemoveAt(0);                // Remove at index
numbers.RemoveRange(2, 3);          // Remove 3 elements starting at index 2

// Searching
int index = numbers.IndexOf(5);             // Index of value, -1 if not found
int lastIndex = numbers.LastIndexOf(5);     // Last index of value
bool contains = numbers.Contains(5);        // Check if exists

// Sorting
List<int> unsorted = new List<int> { 5, 2, 8, 1, 9 };
unsorted.Sort();                      // Sort in place: { 1, 2, 5, 8, 9 }
unsorted.Reverse();                   // Reverse order: { 9, 8, 5, 2, 1 }

// Iterating
foreach (int num in numbers)
{
    Console.WriteLine(num);
}

for (int i = 0; i < colors.Count; i++)
{
    Console.WriteLine($"colors[{i}] = {colors[i]}");
}

// Clear all elements
numbers.Clear();
```

### Working with Dictionary<TKey, TValue>

A dictionary stores key-value pairs, where each key must be unique. Dictionaries provide fast lookups by key, making them ideal for scenarios where you need to quickly find a value based on some identifier.

```csharp
// Creating dictionaries
Dictionary<string, int> ages = new Dictionary<string, int>();
var scores = new Dictionary<string, double>();

// Adding elements
ages.Add("Alice", 30);
ages.Add("Bob", 25);
ages.Add("Charlie", 35);

// Alternative syntax
ages["David"] = 40;  // Adds if key doesn't exist, updates if it does

// Initialize with values
var capitals = new Dictionary<string, string>
{
    { "USA", "Washington D.C." },
    { "UK", "London" },
    { "France", "Paris" }
};

// Accessing values
int aliceAge = ages["Alice"];  // 30
string ukCapital = capitals["UK"];  // "London"

// Safe access with TryGetValue
if (ages.TryGetValue("Eve", out int eveAge))
{
    Console.WriteLine($"Eve's age: {eveAge}");
}
else
{
    Console.WriteLine("Eve not found in dictionary");
}

// Checking existence
bool hasAlice = ages.ContainsKey("Alice");     // true
bool hasAge30 = ages.ContainsValue(30);        // true

// Properties
int count = ages.Count;  // Number of key-value pairs

// Getting all keys or values
var allKeys = ages.Keys;
var allValues = ages.Values;

foreach (string key in ages.Keys)
{
    Console.WriteLine($"Key: {key}");
}

foreach (int value in ages.Values)
{
    Console.WriteLine($"Value: {value}");
}

// Iterating key-value pairs
foreach (KeyValuePair<string, int> pair in ages)
{
    Console.WriteLine($"{pair.Key} is {pair.Value} years old");
}

// Simplified iteration
foreach (var (name, age) in ages)
{
    Console.WriteLine($"{name}: {age}");
}

// Removing elements
ages.Remove("Bob");  // Remove by key
bool removed = ages.Remove("Eve");  // Returns false if key not found

// Updating values
ages["Alice"] = 31;  // Update existing value
```

### Choosing Between Collections

| Scenario | Best Collection |
|----------|----------------|
| Ordered list, frequent additions/removals | `List<T>` |
| Key-value lookups | `Dictionary<TKey, TValue>` |
| Unique values, fast membership testing | `HashSet<T>` |
| First-in-first-out (FIFO) | `Queue<T>` |
| Last-in-first-out (LIFO) | `Stack<T>` |
| Fixed size, best performance | Array |

---

## 15. Enumerations (Enums)

### What are Enums?

An enumeration (enum) is a value type that defines a set of named constants. Enums make code more readable by replacing "magic numbers" with meaningful names. They're particularly useful for representing a fixed set of options, like days of the week, colors, status codes, or any situation where a variable can only take one of a predefined set of values.

```csharp
// Basic enum declaration
enum DayOfWeek
{
    Sunday,
    Monday,
    Tuesday,
    Wednesday,
    Thursday,
    Friday,
    Saturday
}

// Enum with explicit values
enum HttpStatus
{
    OK = 200,
    Created = 201,
    BadRequest = 400,
    Unauthorized = 401,
    NotFound = 404,
    InternalServerError = 500
}

// Enum with different underlying type
enum Permission : byte
{
    None = 0,
    Read = 1,
    Write = 2,
    Delete = 4,
    Admin = 7  // Read | Write | Delete
}
```

By default, enums are based on `int` and values start at 0, incrementing by 1. You can specify different values explicitly. The underlying type can be any integral type (`byte`, `sbyte`, `short`, `ushort`, `int`, `uint`, `long`, `ulong`).

### Using Enums

```csharp
// Declaring enum variables
DayOfWeek today = DayOfWeek.Wednesday;
HttpStatus status = HttpStatus.OK;

// Getting enum values
Console.WriteLine(today);               // "Wednesday"
Console.WriteLine((int)today);          // 3
Console.WriteLine((int)status);         // 200

// Converting to/from int
DayOfWeek day = (DayOfWeek)3;           // Wednesday
int dayValue = (int)DayOfWeek.Friday;   // 5

// Parsing strings
DayOfWeek parsed = Enum.Parse<DayOfWeek>("Monday");  // Monday
bool success = Enum.TryParse<DayOfWeek>("Funday", out DayOfWeek result);

// Checking if value is defined
bool isDefined = Enum.IsDefined(typeof(DayOfWeek), 5);  // true (Friday)
bool isDefined2 = Enum.IsDefined(typeof(DayOfWeek), 10); // false

// Getting all enum values
var allDays = Enum.GetValues<DayOfWeek>();
foreach (var day in allDays)
{
    Console.WriteLine(day);
}

// Getting all enum names
var names = Enum.GetNames<DayOfWeek>();

// Using in switch statements
string GetDayType(DayOfWeek day)
{
    return day switch
    {
        DayOfWeek.Saturday or DayOfWeek.Sunday => "Weekend",
        _ => "Weekday"
    };
}
```

### Flags Enum

When an enum represents a set of flags that can be combined, mark it with the `[Flags]` attribute. This enables bitwise operations and improved string representation for combined values.

```csharp
[Flags]
enum FileAccess
{
    None = 0,
    Read = 1,
    Write = 2,
    Execute = 4,
    All = Read | Write | Execute
}

// Using flags
FileAccess myAccess = FileAccess.Read | FileAccess.Write;
Console.WriteLine(myAccess);  // "Read, Write"

// Checking flags
bool canRead = myAccess.HasFlag(FileAccess.Read);     // true
bool canExecute = myAccess.HasFlag(FileAccess.Execute); // false

// Bitwise operations
FileAccess newAccess = myAccess | FileAccess.Execute;  // Add Execute
FileAccess removed = myAccess & ~FileAccess.Write;      // Remove Write
bool hasReadOrWrite = (myAccess & (FileAccess.Read | FileAccess.Write)) != 0;

// Common pattern for permissions
[Flags]
enum Permissions
{
    None = 0,
    Create = 1 << 0,    // 1
    Read = 1 << 1,      // 2
    Update = 1 << 2,    // 4
    Delete = 1 << 3,    // 8
    
    ReadOnly = Read,
    ReadWrite = Read | Update,
    FullAccess = Create | Read | Update | Delete
}
```

---

## 16. Structs

### What are Structs?

A struct is a value type that can contain data members (fields, properties) and function members (methods). Unlike classes (which are reference types), structs are stored on the stack (in most cases) and are copied by value. Structs are useful for small, simple data structures where value semantics are desired.

```csharp
// Defining a struct
struct Point
{
    public int X;
    public int Y;
    
    // Constructor
    public Point(int x, int y)
    {
        X = x;
        Y = y;
    }
    
    // Method
    public double DistanceTo(Point other)
    {
        int dx = X - other.X;
        int dy = Y - other.Y;
        return Math.Sqrt(dx * dx + dy * dy);
    }
    
    // Override ToString
    public override string ToString() => $"({X}, {Y})";
}

// Using structs
Point p1 = new Point(3, 4);
Point p2 = new Point { X = 6, Y = 8 };

Console.WriteLine(p1);  // "(3, 4)"
Console.WriteLine($"Distance: {p1.DistanceTo(p2)}");  // "Distance: 5"

// Structs are value types - copied on assignment
Point p3 = p1;
p3.X = 100;
Console.WriteLine(p1.X);  // 3 (unchanged)
Console.WriteLine(p3.X);  // 100
```

### When to Use Structs vs Classes

Use structs for:
- Small, simple data structures
- Types that logically represent a single value (like Point, DateTime, TimeSpan)
- Types where value semantics (copy on assignment) are desired
- Types that are short-lived and commonly embedded in other objects

Use classes for:
- Larger, more complex types
- Types that need inheritance
- Types where reference semantics are desired
- Types that need identity (multiple variables can reference the same instance)

```csharp
// Good use of struct - small, value-like
struct Money
{
    public decimal Amount { get; }
    public string Currency { get; }
    
    public Money(decimal amount, string currency)
    {
        Amount = amount;
        Currency = currency;
    }
    
    public Money Add(Money other)
    {
        if (Currency != other.Currency)
            throw new InvalidOperationException("Currencies don't match");
        return new Money(Amount + other.Amount, Currency);
    }
}

// Built-in structs in .NET
DateTime now = DateTime.Now;
TimeSpan duration = TimeSpan.FromHours(2);
Guid id = Guid.NewGuid();
```

---

## 17. Basic File Operations

### Reading and Writing Text Files

The `File` class provides static methods for common file operations, while `StreamReader` and `StreamWriter` offer more control for larger files.

```csharp
using System.IO;

// Write all text at once
File.WriteAllText("output.txt", "Hello, World!");
File.WriteAllLines("lines.txt", new[] { "Line 1", "Line 2", "Line 3" });

// Read all text at once
string content = File.ReadAllText("output.txt");
string[] lines = File.ReadAllLines("lines.txt");

// Append to file
File.AppendAllText("output.txt", "\nAppended line");
File.AppendAllLines("output.txt", new[] { "More", "Lines" });

// Check if file exists
bool exists = File.Exists("output.txt");

// Delete file
if (File.Exists("old.txt"))
{
    File.Delete("old.txt");
}

// Copy and move files
File.Copy("source.txt", "destination.txt");
File.Move("oldname.txt", "newname.txt");

// Get file information
FileInfo info = new FileInfo("output.txt");
Console.WriteLine($"Size: {info.Length} bytes");
Console.WriteLine($"Created: {info.CreationTime}");
Console.WriteLine($"Modified: {info.LastWriteTime}");
```

### Using StreamReader and StreamWriter

For larger files or when you need to process text line by line, use `StreamReader` and `StreamWriter` with the `using` statement for proper resource management.

```csharp
// Writing with StreamWriter
using (StreamWriter writer = new StreamWriter("data.txt"))
{
    writer.WriteLine("Line 1");
    writer.WriteLine("Line 2");
    writer.WriteLine("Line 3");
}

// Reading with StreamReader
using (StreamReader reader = new StreamReader("data.txt"))
{
    string? line;
    while ((line = reader.ReadLine()) != null)
    {
        Console.WriteLine(line);
    }
}

// Modern using statement (C# 8+)
using var writer2 = new StreamWriter("data2.txt");
writer2.WriteLine("Modern syntax");

// Reading until end
using var reader2 = new StreamReader("data.txt");
string allContent = reader2.ReadToEnd();
```

### Working with Directories

```csharp
// Create directory
Directory.CreateDirectory("MyFolder/SubFolder");

// Check if directory exists
bool dirExists = Directory.Exists("MyFolder");

// List files in directory
string[] files = Directory.GetFiles("MyFolder");
string[] textFiles = Directory.GetFiles("MyFolder", "*.txt");
string[] allFiles = Directory.GetFiles("MyFolder", "*", SearchOption.AllDirectories);

// List subdirectories
string[] subdirs = Directory.GetDirectories("MyFolder");

// Delete directory
Directory.Delete("MyFolder", recursive: true);  // Deletes contents too

// Directory info
DirectoryInfo dirInfo = new DirectoryInfo("MyFolder");
Console.WriteLine($"Full path: {dirInfo.FullName}");
Console.WriteLine($"Created: {dirInfo.CreationTime}");

// Get current directory
string currentDir = Directory.GetCurrentDirectory();
Console.WriteLine($"Current: {currentDir}");
```

### Path Operations

```csharp
using System.IO;

// Path manipulation (doesn't require file to exist)
string fullPath = Path.Combine("folder", "subfolder", "file.txt");
// Result: "folder/subfolder/file.txt" (platform-appropriate separator)

string fileName = Path.GetFileName(fullPath);        // "file.txt"
string extension = Path.GetExtension(fullPath);      // ".txt"
string nameWithoutExt = Path.GetFileNameWithoutExtension(fullPath);  // "file"
string directory = Path.GetDirectoryName(fullPath);  // "folder/subfolder"

// Temp paths
string tempFile = Path.GetTempFileName();     // Creates temp file
string tempDir = Path.GetTempPath();          // Temp directory

// Special folders
string docs = Environment.GetFolderPath(Environment.SpecialFolder.MyDocuments);
string desktop = Environment.GetFolderPath(Environment.SpecialFolder.Desktop);
string appData = Environment.GetFolderPath(Environment.SpecialFolder.ApplicationData);

// Check if path is valid
bool isValidPath(string path)
{
    try
    {
        Path.GetFullPath(path);
        return true;
    }
    catch
    {
        return false;
    }
}
```

---

## 18. Best Practices for Beginners

### Naming Conventions

Following consistent naming conventions makes your code readable and professional. In C#, the standard conventions are:

- **PascalCase**: Classes, methods, properties, public fields, enums
  ```csharp
  public class CustomerOrder { }
  public void CalculateTotal() { }
  public string FirstName { get; set; }
  public const int MaxItems = 100;
  ```

- **camelCase**: Local variables, parameters, private fields (often with `_` prefix)
  ```csharp
  int itemCount = 0;
  void ProcessOrder(string orderId) { }
  private string _customerName;
  ```

- **UPPER_CASE**: Constants (though PascalCase is also acceptable)
  ```csharp
  public const double PI = 3.14159;
  ```

### Code Organization

Organize your code logically to make it easier to navigate and maintain:

```csharp
// Within a file, organize members logically:
// 1. Constants and static fields
// 2. Instance fields
// 3. Constructors
// 4. Properties
// 5. Public methods
// 6. Private methods

class Example
{
    // Constants
    public const int MaxSize = 100;
    
    // Private fields
    private int _counter;
    private string _name;
    
    // Constructor
    public Example(string name)
    {
        _name = name;
    }
    
    // Properties
    public string Name => _name;
    
    // Public methods
    public void DoSomething()
    {
        // Implementation
    }
    
    // Private helper methods
    private void HelperMethod()
    {
        // Implementation
    }
}
```

### General Guidelines

1. **Keep methods small and focused**: Each method should do one thing well. If a method is more than 30-50 lines, consider breaking it up.

2. **Use meaningful names**: `CalculateTotalPrice()` is better than `Calc()` or `DoWork()`.

3. **Avoid magic numbers**: Use constants instead of unexplained numbers in code.
   ```csharp
   // Bad
   if (age >= 18) { }
   
   // Good
   const int LegalAdultAge = 18;
   if (age >= LegalAdultAge) { }
   ```

4. **Handle errors gracefully**: Use try-catch for operations that might fail, and provide meaningful error messages.

5. **Comment when necessary**: Write comments to explain "why", not "what". Good code is often self-documenting.

6. **Use var for obvious types**: When the type is clear from context, `var` makes code cleaner. When the type isn't obvious, explicit types improve readability.
   ```csharp
   var customer = new Customer();  // Type is obvious
   var result = GetData();          // Type isn't obvious - use explicit type
   DataResult result = GetData();   // Better
   ```

7. **Format your code consistently**: Use consistent indentation, braces style, and spacing. Visual Studio can format code automatically (Ctrl+K, Ctrl+D).

---

## Summary

This comprehensive guide has covered the fundamentals of C# programming:

- **C# and .NET basics**: Understanding the language, platform, and development environment
- **Program structure**: Namespaces, using directives, statements, and code blocks
- **Variables and data types**: Value types, reference types, and choosing appropriate types
- **Type conversion**: Implicit and explicit conversions, parsing, and safe conversion methods
- **Operators**: Arithmetic, comparison, logical, and assignment operators
- **Control flow**: if/else, switch statements, and expressions
- **Loops**: while, do-while, for, and foreach loops with break and continue
- **Arrays**: Creation, access, multi-dimensional arrays, and array methods
- **Methods**: Defining, parameters, return values, overloading, and expression-bodied methods
- **String manipulation**: Concatenation, interpolation, common methods, and StringBuilder
- **Exception handling**: try-catch-finally and throwing exceptions
- **Console I/O**: Reading input and producing formatted output
- **Collections**: List<T> and Dictionary<TKey, TValue>
- **Enums**: Defining and using enumerations, including flags
- **Structs**: Value types for simple data structures
- **File operations**: Reading, writing, and managing files and directories

These fundamentals provide a solid foundation for learning object-oriented programming and advanced C# features. Practice these concepts by writing small programs that combine different elements, and gradually work on more complex projects to reinforce your understanding.

---

*Created for educational purposes. Made With Love ❤️*
