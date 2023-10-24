# Udemy_Scala_desde_cero

https://superruzafa.github.io/visual-scala-reference/

https://github.com/vadopolski?page=2&tab=repositories

https://www.scala-sbt.org/download.html

## 1. Scala introduction

Scala is a powerful programming language that seamlessly combines object-oriented and functional programming paradigms. Here's a brief introduction:

### Origin:

Scala, short for "scalable language," was created by Martin Odersky and first released in 2003.

It was designed to be concise, elegant, and to address some limitations of Java.

### Object-Oriented and Functional:

Scala is a pure object-oriented language in the sense that every value is an object.

It also incorporates functional programming concepts, allowing developers to write clean and modular code.

### Conciseness:

One of Scala's strengths is its conciseness. It reduces boilerplate code, making it more expressive and readable. 

It's often praised for striking a good balance between brevity and clarity.

### Type System:

Scala has a strong, static type system, which helps catch errors at compile-time rather than runtime. 

It also features type inference, allowing developers to omit certain type annotations.

### Interoperability:

Scala is designed to be fully interoperable with Java. This means you can use Java libraries seamlessly in Scala code, and vice versa. Existing Java codebases can gradually adopt Scala.

### Immutability:

Immutability is encouraged in Scala, contributing to a functional programming style. 

Immutable data structures and immutability by default are key principles in functional programming that Scala embraces.

### Pattern Matching:

Scala includes powerful pattern matching capabilities, which simplifies complex conditional statements and enhances code clarity.

### Concurrency:

Scala supports actor-based concurrency model, inspired by Erlang. 

This makes it well-suited for developing concurrent and distributed systems.

### Scalability:

Scala is designed to be scalable, not just in terms of codebase size but also in supporting parallel and distributed computing.

It can be used for small scripts as well as large systems.

### Tooling:

Scala has a rich set of development tools, including an interactive shell (REPL), build tools like sbt, and support in popular IDEs like IntelliJ IDEA and Eclipse.

In summary, Scala is a versatile language that brings together the best of both object-oriented and functional programming worlds. 

Its interoperability with Java and focus on conciseness make it a compelling choice for a wide range of applications.

### First Scala sample:

Let's create a simple example that incorporates some of Scala's features. 

We'll create a program that calculates the factorial of a number using recursion, immutability, pattern matching, and type inference.

```scala
// Object-Oriented and Functional: Define a class with a companion object
class FactorialCalculator {
  // Immutable data: Use val for immutable variables
  def factorial(n: Int): Int = {
    if (n <= 0) 1
    else n * factorial(n - 1)
  }
}

// Companion object for the class with a main method
object FactorialCalculator {
  // Type inference: Scala infers the return type of the method
  def main(args: Array[String]): Unit = {
    // Immutable data: Use val for immutable variables
    val number = 5

    // Pattern matching: Match on the result of factorial calculation
    val result = number match {
      case 0 => 1
      case _ => new FactorialCalculator().factorial(number)
    }

    // Output the result
    println(s"The factorial of $number is $result")
  }
}
```

In this example:

**Object-Oriented and Functional**: We define a class FactorialCalculator to encapsulate the logic for calculating factorial.

**Immutable Data**: We use val for immutable variables, like number.

**Type Inference**: The return type of the factorial method is not explicitly declared; Scala infers it.

**Pattern Matching**: We use pattern matching in the match block to handle different cases, including the base case where the number is 0.

**Interoperability**: Although we didn't explicitly use Java libraries in this example, Scala can easily interoperate with Java libraries.

**Scalability**: This example is simple, but Scala's features make it suitable for building larger and more complex systems.

Feel free to run this Scala code in an environment that supports Scala, and you should see the factorial of 5 printed to the console.

## 2. Main differences between Scala and Java

Here are some basic differences between Scala and Java:

**Paradigm:**

Java: Primarily an object-oriented programming language with support for procedural programming.

Scala: Combines object-oriented and functional programming paradigms.

**Type System:**

Java: Has a more verbose type system. Requires explicit type annotations in many cases.

Scala: Employs a more concise and expressive type system. Type inference reduces the need for explicit type annotations.

**Syntax:**

Java: Generally more verbose syntax.

Scala: Emphasizes conciseness and expressive syntax. Less boilerplate code.

**Immutability:**

Java: Immutability needs to be explicitly enforced, and Java has mutable and immutable classes.

Scala: Favors immutability by default. Immutable data structures are encouraged.

**Null Handling:**

Java: Null is a valid value for any reference type, leading to the possibility of NullPointerExceptions.

Scala: Introduces the Option type to handle nullability more safely. Null references are less common.

**Concurrency:**

Java: Primarily relies on thread-based concurrency using classes like Thread and Runnable. 

Java introduced the java.util.concurrent package for improved concurrency.

Scala: Utilizes the Actor model for concurrency.

Actors are lightweight, and immutability helps in writing concurrent and parallel code.

**Pattern Matching:**

Java: Traditional switch statements are limited and cannot match complex patterns.

Scala: Employs powerful pattern matching constructs for expressive and concise code.

**Interoperability:**

Java: Designed to be highly interoperable with other Java code. Can easily use Java libraries.

Scala: Fully interoperable with Java. Scala code can call Java methods and use Java libraries seamlessly.

**Tooling:**

Java: Mature ecosystem with robust IDE support (Eclipse, IntelliJ IDEA, etc.) and build tools (Maven, Gradle).

Scala: Good IDE support (IntelliJ IDEA, Eclipse with Scala IDE) and build tools like sbt.

**Learning Curve:**

Java: Generally considered more straightforward for beginners due to its simpler syntax.

Scala: Has a steeper learning curve, especially for those new to functional programming concepts.

However, it can lead to more expressive and concise code once mastered.

These differences highlight the unique features and design principles of each language.

While Java remains a dominant language in the industry, Scala offers a more expressive and scalable alternative, especially for those interested in functional programming.


## 3. Scala web pages

https://docs.scala-lang.org/

https://docs.scala-lang.org/getting-started/index.html

https://docs.scala-lang.org/tour/tour-of-scala.html

## 4. Scala download

https://www.scala-lang.org/download/

## 5. Scala installation



## 6. IntelliJ installation (Commnunity edition)



## 7.How to create a Scala project in IntelliJ



## 8. Introduction to REPL. Command tools

Let's delve into Scala's **REPL (Read-Eval-Print Loop)** and command-line tools.

REPL (Read-Eval-Print Loop): Scala's REPL is an interactive shell that allows you to execute Scala code one line at a time:

**Read:** The REPL reads your input line by line.

**Eval:** It evaluates the expression you entered.

**Print:** It prints the result of the evaluation.

**Loop:** The process repeats, creating an interactive and iterative development environment.

To start the REPL, open your terminal and type scala. 

You'll enter an interactive session where you can directly write and execute Scala code.

```
scala> val x = 10
x: Int = 10
```

```
scala> println(x * 2)
20
```

You can use the REPL for quick experimentation, testing small code snippets, or exploring the language features.

**Command-Line Tools:**

Scala comes with several command-line tools that facilitate various tasks:

**scalac:** The Scala compiler. It compiles Scala source code into Java bytecode.

```bash
# Compile a Scala file
scalac MyFile.scala
```

**Run the compiled bytecode**
scala MyFile

**scaladoc:** Generates HTML documentation from Scala source code.

```bash
# Generate documentation
scaladoc MyFile.scala
```

**scalap:** Decompiles Scala classes back to source code.

```bash
# Decompile a class file
scalap MyFile.class
```

**sbt (Scala Build Tool):** While not a command-line tool bundled with Scala, sbt is commonly used for managing Scala projects, compiling, testing, and more.

```bash
# Run sbt in interactive mode
sbt
```

These tools empower you to manage your Scala codebase efficiently, from compiling and testing to generating documentation.

## 9. Data types

Scala is a statically-typed language, which means that the type of a variable is known at compile time. Here are some basic data types in Scala:

**Integers:**

Int: 32-bit signed integer.

Long: 64-bit signed integer.

Short: 16-bit signed integer.

Byte: 8-bit signed integer.

```scala
val x: Int = 42
val y: Long = 123456789L
```

**Floating Point Numbers:**

Float: 32-bit single-precision floating point.

Double: 64-bit double-precision floating point.

```scala
val a: Float = 2.5f
val b: Double = 3.14
```

**Characters and Strings:**

Char: 16-bit Unicode character.

String: A sequence of characters.

```scala
val char: Char = 'A'
val str: String = "Hello, Scala!"
```

**Boolean:**

Boolean: Represents true or false.

```scala
Copy code
val isScalaAwesome: Boolean = true
```

**Tuples:**

A grouping of values of different types.

```scala
val tuple: (Int, String, Double) = (1, "Scala", 3.14)
```

**Arrays:**

A mutable sequence of elements of the same type.

```scala
val array: Array[Int] = Array(1, 2, 3, 4, 5)
```

**Lists:**

An immutable linked list.

```scala
val list: List[Int] = List(1, 2, 3, 4, 5)
```

**Maps:**

A collection of key-value pairs.

```scala
val map: Map[String, Int] = Map("one" -> 1, "two" -> 2, "three" -> 3)
```

**Option:**

Represents a value that may or may not be present.

```scala
val maybeValue: Option[Int] = Some(42)
```

These are just the basics. Scala also supports more advanced types, and it has a strong type inference system, allowing you to omit types in many cases where the compiler can infer them.

## 10. Var y Val. Variables.

In Scala, val and var are used to declare variables, but they have different characteristics:

### val (Immutable Variable):

Once a val is assigned, its value cannot be changed. It's similar to declaring a constant.

```scala
Copy code
val pi: Double = 3.14
val greeting: String = "Hello, Scala!"

// Attempting to reassign will result in a compilation error:
// pi = 3.14159  // Compilation error
The values assigned to val are immutable.
```

### var (Mutable Variable):

A var can have its value reassigned. It's a mutable variable.

```scala
Copy code
var counter: Int = 0

// Value can be changed:
counter = 1
```

While using var provides mutability, it's generally considered good practice to use val whenever possible to make your code more robust and functional.

Here's a simple example using both val and var:

```scala
// Immutable variable
val fixedValue: String = "I won't change"

// Mutable variable
var changingValue: Int = 42

// Let's do some changes
changingValue = 100

// The following line will result in a compilation error
// fixedValue = "Oops, I tried to change"

// Output the values
println(fixedValue)
println(changingValue)
```

In this example, fixedValue cannot be reassigned, while changingValue can be modified. 

It's a good practice to use val by default and only use var when necessary for specific scenarios where mutability is required.

## 11. Create variable in lazy mode

In Scala, you can create variables in lazy mode using the **lazy** keyword.

A lazy variable is only evaluated when it is accessed for the first time, and its value is then cached for future use. 

This can be useful for delaying the initialization of expensive operations or computations until they are actually needed.

```scala
object LazyExample extends App {
  // Define a lazy variable
  lazy val expensiveOperation: String = {
    println("Executing expensive operation")
    "Result of expensive operation"
  }

  // The expensive operation is not executed yet

  // Access the lazy variable
  println("Accessing lazy variable:")
  println(expensiveOperation)
  
  // Since the lazy variable has been accessed, the expensive operation is now executed
}
```

In this example, the expensiveOperation is a lazy variable.

The actual execution of the code inside the lazy val is deferred until the variable is accessed.

When you run this program, you'll see that the "Executing expensive operation" message is only printed when the expensiveOperation variable is accessed for the first time.

This lazy evaluation can be beneficial in situations where you want to avoid unnecessary computations until the value is actually needed.

## 12. Variables and constants practices

Scala is a powerful language that combines object-oriented and functional programming features. 

Let's dive into some advanced practices for variables and constants in Scala:

## Variables:

## Mutable Variables (var):

```scala
var counter: Int = 10
counter += 1
```

Type Inference:

```scala
var message = "Hello, Scala!" // Compiler infers the type
```

## Variable Scope:

```scala
def printCounter(): Unit = {
  var innerCounter = 5
  println(innerCounter)
}
```

## Lazy Evaluation:

```scala
lazy val expensiveOperation: Int = {
  // Some expensive computation
  42
}
```

## Constants:

## Immutable Variables (val):

```scala
Copy code
val pi: Double = 3.14
```

**Case Classes:**

```scala
case class Point(x: Int, y: Int)
val origin = Point(0, 0)
```

## 13. Comments

## 14. Blocks

## 15. Operators

## 16. Conditions. IF command

## 17. Loops

In Scala, there are different ways to implement loops. Let me show you a couple of examples.

### For Loop:

The for loop in Scala is similar to loops in other languages. It iterates over a range of values or a collection.

```scala
// Example 1: Looping through a range of values
for (i <- 1 to 5) {
  println(s"Value of i: $i")
}

// Example 2: Looping through a collection
val fruits = List("apple", "banana", "orange")
for (fruit <- fruits) {
  println(s"Current fruit: $fruit")
}
```

### While Loop:

Scala also supports the traditional while loop.

```scala
// Example: While loop
var x = 0
while (x < 5) {
  println(s"Value of x: $x")
  x += 1
}
```

### Do-While Loop:

The do-while loop ensures that the block of code is executed at least once before checking the condition.

```scala
// Example: Do-while loop
var y = 0
do {
  println(s"Value of y: $y")
  y += 1
} while (y < 5)
```

### Functional Approach - For Each:

Scala encourages a functional programming style, and you can often use higher-order functions like foreach to achieve looping behavior.

```scala
Copy code
// Example: Using foreach with a collection
val numbers = List(1, 2, 3, 4, 5)
numbers.foreach { num =>
  println(s"Current number: $num")
}
```

## 18. Ranges

## 19. Default variables initialization

## 20. Pattern Matching part 1

## 21. Pattern Matching part 2

## 22. Numbers

## 23. Collections

The following figure shows all collections in package scala.collection. These are all high-level abstract classes or traits, which generally have mutable as well as immutable implementations.

![image](https://github.com/luiscoco/Udemy_Scala_desde_cero/assets/32194879/ebf7b100-f86f-43c6-9875-1a69bc6374b3)

The following figure shows all collections in package scala.collection.immutable.

![image](https://github.com/luiscoco/Udemy_Scala_desde_cero/assets/32194879/19c430d3-f3f6-46cf-a9c5-c0abe910bf7f)

And the following figure shows all collections in package scala.collection.mutable.

![image](https://github.com/luiscoco/Udemy_Scala_desde_cero/assets/32194879/fa21af93-e143-43d2-89f4-e76cf6dfa5aa)

## 24. List

## 25. List operations

## 26. More operations with List

## 27. ListBuffer

## 28. Array

## 29. ArrayBuffer

## 30. Set

## 31. Map

## 32. Functions

## 33. Procedures. Functions that do not return a value

## 34. Functions with parameters

## 35. Named parameters

## 36. Default parameters

## 37. Variable number of paramters

## 38. How to create an application with IntelliJ IDEA

## 39. My first application with Scala

## 40. Crear una aplicación con el método "main".

## 41. Compile with scalac

## 42. Clases Parte 1.

## 43. Clases Parte 2.

## 44. Herencia.

## 45. Traits Parte 1.

## 46. Traits Parte 2.

## 47. Traits Múltiples.

## 48. Modificadores de acceso: private, public, protected.

## 49. Constructores.

## 50. Constructores auxiliares.

## 51. Constructores múltiples.

## 52. Singleton Objects.

## 53. Companion Objects.

## 54. Crear Instancias son NEW.

## 55. Case Class.

## 56. Clases Abstractas.

# Programación funcional.

## 57. High Order Functrions.

## 58. Funciones anónimas. Functions literals.

## 59. Funciones con parámetros.

## 60. Funciones como variable.

## 61. Devolver una función.

## 62. Partially Applied Functions.

## 63. Currying Functions.

## 64. Closures.

## 65. Options.

## 66. Exceptions. Try Catch.

## 67. Exceptions, finally.

## 68. Exceptions, Throw.

## 69. Sobrecarga. Overloading.

## 70. Leer ficheros de texto.

71. Escribir y leer ficheros binarios.
