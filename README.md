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

![image](https://github.com/luiscoco/Udemy_Scala_desde_cero/assets/32194879/014cd787-48d9-4e34-97db-1fd03df9bb58)

## 6. IntelliJ installation (Commnunity edition)

https://www.jetbrains.com/idea/

https://www.jetbrains.com/idea/download/?section=windows

https://www.jetbrains.com/idea/download/download-thanks.html?platform=windows&code=IIC

![image](https://github.com/luiscoco/Udemy_Scala_desde_cero/assets/32194879/16dbcc15-a1bd-46f0-82d4-034d18819b8b)

## 7.How to create a Scala project in IntelliJ

https://docs.scala-lang.org/getting-started/intellij-track/getting-started-with-scala-in-intellij.html

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

In Scala, comments are used to add explanatory notes or annotations to the code. 

There are two types of comments in Scala: single-line comments and multi-line comments.

### Single-line comments:

Single-line comments start with // and continue until the end of the line. Anything following // on that line is treated as a comment and is ignored by the Scala compiler.

```scala
// This is a single-line comment
val x = 42  // You can also add a comment at the end of a line of code
```

### Multi-line comments:

Multi-line comments begin with /* and end with */. Everything between these delimiters is treated as a comment.

```scala
/*
This is a
multi-line comment
*/
val y = 10
```

Here's an example that combines both types of comments:

```scala
// This is a single-line comment

/*
  This is a multi-line comment
  spanning multiple lines
*/

val z = 3 // Another single-line comment
```

Comments are useful for documenting your code, providing explanations for complex logic, or temporarily disabling code for testing purposes.

## 14. Blocks

In Scala, "blocks" usually refer to a sequence of expressions enclosed in curly braces {}. 

These blocks can be used in various contexts, such as defining a code block for a function, conditionals, loops, or even just a standalone block.

### Code Block:

```scala
// defining a block for a function
def greet(name: String): Unit = {
  println(s"Hello, $name!")
}

// using the function with a block
greet("Alice")
```

### Conditional Block:

```scala
// defining a block for if-else
val x = 10
if (x > 5) {
  println("x is greater than 5")
} else {
  println("x is 5 or less")
}
```

### Loop Block:

```scala
// defining a block for a loop
for (i <- 1 to 5) {
  println(s"Number $i")
}
```

### Standalone Block:

```scala
// a standalone block
val result = {
  val a = 10
  val b = 5
  a + b
}
println(s"Result: $result")
```

In each case, the curly braces {} contain a block of code, and the expressions inside are executed in sequence. 

It's important to note that the last expression in the block is the value of the block. In the fourth example, the value of the block is a + b, which is assigned to the result variable.

## 15. Operators

In Scala, operators are special symbols that represent computations involving one or more operands. 

Let me give you some examples of commonly used operators in Scala:

#### Arithmetic Operators:

+ (addition)
- (subtraction)
* (multiplication)
/ (division)
% (modulo)

```scala
val sum = 5 + 3
val difference = 7 - 2
val product = 4 * 6
val quotient = 10 / 2
val remainder = 15 % 4
```

#### Relational Operators:

== (equal to)
!= (not equal to)
< (less than)
> (greater than)
<= (less than or equal to)
>= (greater than or equal to)

```scala
val isEqual = 5 == 5
val notEqual = 10 != 3
val lessThan = 8 < 12
val greaterThan = 15 > 9
val lessThanOrEqual = 20 <= 20
val greaterThanOrEqual = 25 >= 18
```

#### Logical Operators:

&& (logical AND)
|| (logical OR)
! (logical NOT)

```scala
val andResult = (true && false)
val orResult = (true || false)
val notResult = !true
```

#### Bitwise Operators:

& (bitwise AND)
| (bitwise OR)
^ (bitwise XOR)
<< (left shift)
>> (right shift)
>>> (unsigned right shift)

```scala
val bitwiseAnd = 5 & 3
val bitwiseOr = 5 | 3
val bitwiseXor = 5 ^ 3
val leftShift = 8 << 2
val rightShift = 16 >> 2
```

Let's delve into some more advanced topics related to operators in Scala:

#### Pattern Matching:

Scala has a powerful feature called pattern matching, which can be used as a more flexible and powerful alternative to traditional switch statements in other languages. It allows you to match complex patterns and destructure data.

```scala
val day = "Monday"

val result = day match {
  case "Monday" => "Start of the week"
  case "Friday" | "Saturday" | "Sunday" => "Weekend"
  case _ => "Midweek blues"
}
```

In this example, the match expression checks the value of day against different patterns and produces a result accordingly.

#### Operator Overloading:

Scala supports operator overloading, which means you can define your own meaning for operators when used with instances of your classes. 

This is achieved by defining methods with symbolic names.

```scala
class Complex(real: Double, imaginary: Double) {
  def +(that: Complex): Complex =
    new Complex(this.real + that.real, this.imaginary + that.imaginary)

  override def toString: String = s"$real + ${imaginary}i"
}

val c1 = new Complex(1.0, 2.0)
val c2 = new Complex(2.0, 3.0)
val sum = c1 + c2
println(sum)  // Output: 3.0 + 5.0i
```

Here, the + operator is overloaded to perform addition of two Complex instances.

#### Infix Notation:

In Scala, methods that take a single parameter can be used with infix notation. 

This allows you to write expressive and readable code.

```scala
class Person(name: String) {
  def says(message: String): String = s"$name says: $message"
}

val john = new Person("John")
val greeting = john says "Hello, Scala!"
```

The says method is used in infix notation here, making the code read like a sentence.

#### Type-Safe Equality:

In Scala, you can use == for structural equality and eq for reference equality. 

The == operator is type-safe and avoids some common pitfalls present in other languages.

```scala
val x: Int = 5
val y: String = "5"

// Type-safe equality
val isEqual: Boolean = x == 5  // true
val isNotEqual: Boolean = x == y  // false
```

It's generally recommended to use == for equality comparisons.

## 16. Conditions. IF command

In Scala, the if statement is used for conditional commands. It allows you to execute a block of code if a certain condition is true. 

The basic syntax looks like this:

```scala
if (condition) {
  // code to be executed if the condition is true
} else {
  // code to be executed if the condition is false
}
```

Here's a simple example:

```scala
val x = 10

if (x > 5) {
  println("x is greater than 5")
} else {
  println("x is not greater than 5")
}
```

In this example, if the value of x is greater than 5, it will print "x is greater than 5"; otherwise, it will print "x is not greater than 5."

You can also use the else if clause to check multiple conditions:

```scala
val y = 7

if (y > 10) {
  println("y is greater than 10")
} else if (y > 5) {
  println("y is greater than 5 but not greater than 10")
} else {
  println("y is 5 or less")
}
```

This structure allows you to check a series of conditions, and the first one that is true will execute its corresponding block of code.

Additionally, you can use the val result = if (condition) expr1 else expr2 syntax for assigning values based on a condition:

```scala
val result = if (x > 5) "x is greater than 5" else "x is not greater than 5"
println(result)
```

In this case, the result variable will hold the string based on whether the condition is true or false.

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

In Scala, a range is an ordered sequence of numbers. 

You can create ranges using the to and until methods. 

The to method creates an inclusive range, while the until method creates a range that excludes the upper bound.

### Inclusive Range (to):

```scala
val inclusiveRange = 1 to 5
// Result: Range(1, 2, 3, 4, 5)
```

This creates a range from 1 to 5 (inclusive).

### Exclusive Range (until):

```scala
val exclusiveRange = 1 until 5
// Result: Range(1, 2, 3, 4)
```

This creates a range from 1 to 4 (excluding 5).

### Specifying a Step:

```scala
val steppedRange = 1 to 10 by 2
// Result: Range(1, 3, 5, 7, 9)
```

Here, the by method is used to specify the step, so the range goes up by 2.

### Creating a Range of Characters:

```scala
val charRange = 'a' to 'z'
// Result: NumericRange(a, b, c, ..., z)
```

Ranges aren't limited to numbers; you can create ranges of characters as well.

### Using Range in a Loop:

```scala
for (i <- 1 to 3) {
  println(s"Value of i: $i")
}
```

```
// Output:
// Value of i: 1
// Value of i: 2
// Value of i: 3
```

Ranges are often used in for loops to iterate over a sequence of values.

Ranges in Scala are quite versatile and can be used in various situations where you need a sequence of ordered values.

## 19. Default variables initialization

in Scala, you can initialize variables with default values when you declare them. 

This is handy when you want to ensure that a variable always has a meaningful value, even if it's not explicitly set by the programmer.

```scala
// Example 1: Initializing an Int with a default value
var count: Int = _

println(s"Count: $count") // Prints: Count: 0 (default value for Int)

// Example 2: Initializing a String with a default value
var name: String = _

println(s"Name: $name") // Prints: Name: null (default value for String)

// Example 3: Initializing a custom class with a default value
class Person(var name: String = "Unknown", var age: Int = 0)

val defaultPerson = new Person()
println(s"Default Person - Name: ${defaultPerson.name}, Age: ${defaultPerson.age}")
// Prints: Default Person - Name: Unknown, Age: 0
```

In these examples:

In Example 1, count is an Int variable initialized with the default value of 0.

In Example 2, name is a String variable initialized with the default value of null.

In Example 3, a Person class is defined with default values for its parameters. 

When creating a new Person without specifying values, it takes the default values.

Default values make your code more robust by ensuring that variables have meaningful initial values, reducing the chance of unexpected behavior due to uninitialized variables.

## 20. Pattern Matching part 1

 In Scala, pattern matching is a powerful feature that allows you to match complex data structures and perform different actions based on the structure of the data. 
 
 It's often used as a more powerful and readable alternative to traditional switch statements.

### Example 1: Matching on Values

```scala
def describe(x: Any): String = x match {
  case 1 => "One"
  case "hello" => "Greeting"
  case true => "True"
  case _ => "Something else"
}

val result = describe("hello")
println(result)  // Output: Greeting
```

In this example, the describe function takes any input (x) and matches it against different cases.

If x is equal to 1, it returns "One."

If it's equal to "hello," it returns "Greeting."

If it's true, it returns "True."

If none of these cases match, it returns "Something else."

### Example 2: Matching on Types

```scala
def process(x: Any): String = x match {
  case i: Int => s"Received an integer: $i"
  case s: String => s"Received a string: $s"
  case _ => "Unknown type"
}

val result1 = process(42)
val result2 = process("Scala")

println(result1)  // Output: Received an integer: 42
println(result2)  // Output: Received a string: Scala
```

Here, the process function matches based on the type of the input. 

If it's an Int, it prints a message with the integer value. 

If it's a String, it prints a message with the string value. 

If it doesn't match any of these cases, it prints "Unknown type."

### Example 3: Matching on Case Classes

```scala
case class Person(name: String, age: Int)

def greet(person: Person): String = person match {
  case Person("Alice", 25) => "Hi Alice!"
  case Person("Bob", 30) => "Hello Bob!"
  case Person(name, age) => s"Nice to meet you, $name (age $age)!"
}

val alice = Person("Alice", 25)
val bob = Person("Bob", 30)
val unknown = Person("Unknown", 40)

println(greet(alice))    // Output: Hi Alice!
println(greet(bob))      // Output: Hello Bob!
println(greet(unknown))  // Output: Nice to meet you, Unknown (age 40)!
```

In this example, the greet function matches on instances of the Person case class. 

It checks if the person is Alice or Bob and responds accordingly. 

If it's neither Alice nor Bob, it provides a generic greeting.

These are just a few examples of pattern matching in Scala. 

It's a versatile feature that can be used in various contexts, making your code more expressive and concise.

## 21. Pattern Matching part 2

Let's delve into some more advanced concepts of pattern matching in Scala.

### Example 4: Matching Lists

Pattern matching can be applied to collections like Lists. Here's an example:

```scala
def listMatch(lst: List[Int]): String = lst match {
  case Nil => "Empty list"
  case head :: tail => s"Head: $head, Tail: $tail"
}

val myList = List(1, 2, 3, 4, 5)
val emptyList = List.empty[Int]

println(listMatch(myList))      // Output: Head: 1, Tail: List(2, 3, 4, 5)
println(listMatch(emptyList))   // Output: Empty list
```

In this example, the listMatch function matches a list. 

If it's an empty list (Nil), it returns "Empty list." 

If it has at least one element, it deconstructs the list into the head and tail and prints them.

### Example 5: Matching with Guards

You can use guards to add conditions to your pattern matches:

```scala
def describe(x: Any): String = x match {
  case i: Int if i > 0 => "Positive integer"
  case i: Int if i < 0 => "Negative integer"
  case s: String if s.length > 5 => "Long string"
  case _ => "Other"
}

val result1 = describe(42)
val result2 = describe(-10)
val result3 = describe("Scala is awesome!")

println(result1)  // Output: Positive integer
println(result2)  // Output: Negative integer
println(result3)  // Output: Long string
```

Here, the patterns are matched with additional conditions (if i > 0, if i < 0, if s.length > 5).

It allows you to filter the matched cases based on specified conditions.

### Example 6: Pattern Matching in for Comprehensions

Pattern matching can also be used in for comprehensions for extracting values:

```scala
val listOfEithers: List[Either[String, Int]] = List(Right(42), Left("Error"), Right(99))

val result = for {
  Right(num) <- listOfEithers
} yield num

println(result)  // Output: List(42, 99)
```

Here, the for comprehension iterates over a list of Either values.

The pattern Right(num) is used to extract values from Right instances, effectively filtering out Left instances.

### Example 7: Sealed Traits and Pattern Matching

Sealed traits are often used in combination with pattern matching. 

A sealed trait can only be extended by classes in the same file, which allows exhaustive pattern matching:

```scala
sealed trait Shape
case class Circle(radius: Double) extends Shape
case class Rectangle(width: Double, height: Double) extends Shape
case object UnknownShape extends Shape

def area(shape: Shape): Double = shape match {
  case Circle(r) => math.Pi * r * r
  case Rectangle(w, h) => w * h
  case UnknownShape => 0.0
}

val circle = Circle(5.0)
val rectangle = Rectangle(3.0, 4.0)
val unknown = UnknownShape

println(area(circle))      // Output: 78.53981633974483
println(area(rectangle))   // Output: 12.0
println(area(unknown))     // Output: 0.0
```

Here, the Shape trait is sealed, and we have two case classes (Circle and Rectangle) and an object (UnknownShape) extending it. 

The area function uses pattern matching to calculate the area based on the shape.

## 22. Numbers

Scala is a versatile programming language that combines object-oriented and functional programming paradigms. 

Let's dive into some basic concepts using examples with numbers in Scala.

### Declaring Variables:

In Scala, you can declare variables using val for immutable values (constants) and var for mutable variables.

```scala
val x: Int = 5 // Immutable variable
var y: Double = 3.14 // Mutable variable
```

### Basic Arithmetic Operations:

Scala supports standard arithmetic operations on numbers.

```scala
val sum = x + y
val difference = x - y
val product = x * y
val quotient = x / y
```

### Data Types:

Scala has various numeric data types, such as Int, Double, Float, Long, etc.

```scala
Copy code
val intNumber: Int = 10
val doubleNumber: Double = 3.5
val floatNumber: Float = 2.0f
val longNumber: Long = 1000000000L
```

### Type Inference:

Scala has a powerful type inference system, so you don't always need to explicitly mention the data type.

```scala
val a = 10 // Scala infers that 'a' is of type Int
val b = 3.5 // Scala infers that 'b' is of type Double
```

### Math Functions:

Scala provides various math functions that you can use on numbers.

```scala
val absoluteValue = math.abs(-10)
val squareRoot = math.sqrt(25)
val power = math.pow(2, 3)
```

### Ranges:

Scala has a convenient way to create ranges of numbers.

```scala
val range = 1 to 5 // Represents the range 1, 2, 3, 4, 5
```

### Collections:

Scala has powerful collection types like Lists, Arrays, etc., which can store and manipulate sequences of numbers.

```scala
val numbersList = List(1, 2, 3, 4, 5)
val squaredNumbers = numbersList.map(x => x * x)
```

These are just a few examples to give you a taste of working with numbers in Scala. 

The language has a lot more features and capabilities, especially when it comes to functional programming constructs and concise syntax.


## 23. Collections

The following figure shows all collections in package scala.collection. These are all high-level abstract classes or traits, which generally have mutable as well as immutable implementations.

![image](https://github.com/luiscoco/Udemy_Scala_desde_cero/assets/32194879/ebf7b100-f86f-43c6-9875-1a69bc6374b3)

### Inmutable collections

The following figure shows all collections in package scala.collection.immutable.

![image](https://github.com/luiscoco/Udemy_Scala_desde_cero/assets/32194879/19c430d3-f3f6-46cf-a9c5-c0abe910bf7f)

In Scala, immutable collections are collections whose elements and size cannot be changed after they are created. 

Here are some examples of immutable collections in Scala:

#### List:

```scala
// Creating an immutable list
val immutableList = List(1, 2, 3)

// Adding elements creates a new list
val newList = immutableList :+ 4
```

#### Set:

```scala
// Creating an immutable set
val immutableSet = Set(1, 2, 3)

// Adding elements creates a new set
val newSet = immutableSet + 4
```

#### Map:

```scala
// Creating an immutable map
val immutableMap = Map("a" -> 1, "b" -> 2, "c" -> 3)

// Adding key-value pairs creates a new map
val newMap = immutableMap + ("d" -> 4)
```

#### Vector:

```scala
// Creating an immutable vector
val immutableVector = Vector(1, 2, 3)

// Adding elements creates a new vector
val newVector = immutableVector :+ 4
```

#### Tuple:

```scala
// Creating an immutable tuple
val immutableTuple = (1, "Hello", 3.14)

// Extracting values from a tuple
val (first, second, third) = immutableTuple
```

In all these examples, notice that operations that seem to modify the collection actually return a new instance of the collection with the desired changes, leaving the original collection unchanged. 

This immutability is a key feature for functional programming in Scala and helps in writing more predictable and thread-safe code.


### Mutable collections

And the following figure shows all collections in package scala.collection.mutable.

![image](https://github.com/luiscoco/Udemy_Scala_desde_cero/assets/32194879/fa21af93-e143-43d2-89f4-e76cf6dfa5aa)

In Scala, mutable collections provide a way to modify, add, or remove elements. Here are some examples:

#### Lists:

```scala
Copy code
import scala.collection.mutable.ListBuffer

// Create a mutable ListBuffer
val mutableList = ListBuffer(1, 2, 3)

// Add elements to the ListBuffer
mutableList += 4
mutableList ++= List(5, 6)

// Remove elements from the ListBuffer
mutableList -= 2

// Print the mutable list
println(mutableList)
```

#### Sets:

```scala
import scala.collection.mutable.HashSet

// Create a mutable HashSet
val mutableSet = HashSet(1, 2, 3)

// Add elements to the HashSet
mutableSet += 4
mutableSet ++= Set(5, 6)

// Remove elements from the HashSet
mutableSet -= 2

// Print the mutable set
println(mutableSet)
```

#### Maps:
```scala
import scala.collection.mutable.HashMap

// Create a mutable HashMap
val mutableMap = HashMap("a" -> 1, "b" -> 2, "c" -> 3)

// Add key-value pairs to the HashMap
mutableMap += ("d" -> 4)
mutableMap ++= Map("e" -> 5, "f" -> 6)

// Remove key-value pairs from the HashMap
mutableMap -= "b"

// Print the mutable map
println(mutableMap)
```

These examples use ListBuffer, HashSet, and HashMap from the mutable package in Scala. 

Remember, while mutable collections offer flexibility, it's generally recommended to use immutable collections whenever possible to avoid unexpected side effects in your code.

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



## 40. Create an application including the "main" method




## 41. Compile with scalac




## 42. Clases Part 1

In Scala, classes are a fundamental building block of object-oriented programming.

They serve as blueprints for creating objects, which are instances of those classes. Here's a brief overview:

### Class Definition:

```scala
class MyClass {
  // class body
}
```

### Constructor:

You can have a primary constructor in the class definition itself.

Parameters of the primary constructor are used to initialize the class fields.

```scala
class Person(name: String, age: Int) {
  // class body
}
```

### Fields:

Fields are variables that hold data for each object created from the class.

In Scala, fields are automatically created from the parameters of the primary constructor.

```scala
class Person(name: String, age: Int) {
  val personName: String = name
  var personAge: Int = age
}
```

### Methods:

Methods are functions defined within the class.

They can operate on the class fields and perform various tasks.

```scala
class Person(name: String, age: Int) {
  def sayHello(): Unit = {
    println(s"Hello, my name is $name and I'm $age years old.")
  }
}
```

### Object Instantiation:

You create objects from classes using the new keyword.

```scala
val person = new Person("John", 25)
```

### Inheritance:

Scala supports single-class inheritance using the extends keyword.

```scala
class Student(name: String, age: Int, studentId: String) extends Person(name, age) {
  // additional fields and methods for Student
}
```

###  Overriding Methods:

You can override methods from a parent class in a child class using the override keyword.

```scala
override def sayHello(): Unit = {
  println(s"Hello, I'm a student named $name.")
}
```

### Case Classes:

Scala has a special kind of class called a case class, which is often used for immutable data.

```scala
case class Point(x: Int, y: Int)
```

Case classes automatically provide methods like equals, toString, and hashCode.

That's a quick overview! Classes in Scala offer a powerful way to structure your code in an object-oriented manner.

## 43. Clases Part 2

Scala, being a versatile language, offers several advanced features related to classes and object-oriented programming. Let's dive into a few more advanced topics:

### Companion Objects:

In Scala, a companion object is an object with the same name as a class.

It is often used for defining factory methods or other methods that are not specific to instances of the class.

```scala
class MyClass(value: Int)

object MyClass {
  def createInstance(value: Int): MyClass = new MyClass(value)
}
```

### Case Classes (Deeper):

Case classes not only provide convenience methods but also automatically generate a companion object with apply methods for easy instantiation.

```scala
case class Person(name: String, age: Int)
val person = Person("John", 25)  // Automatically calls apply method in the companion object
```

Case classes also generate copy methods for easy creation of modified copies.

```scala
val olderPerson = person.copy(age = 30)
```

### Sealed Classes and Pattern Matching:

A sealed class can only be extended in the same file. This allows exhaustive pattern matching.

```scala
sealed abstract class Result
case class Success(message: String) extends Result
case class Failure(reason: String) extends Result

def processResult(result: Result): Unit = result match {
  case Success(msg) => println(s"Success: $msg")
  case Failure(reason) => println(s"Failure: $reason")
}
```

### Type Parameterization (Generics):

You can parameterize classes with types, making them generic.

```scala
class Box[A](value: A)

val intBox = new Box(42)
val stringBox = new Box("Hello")
```

### Self Types:

Self types express limitations on who can instantiate a class.

```scala
trait Logger {
  def log(message: String): Unit
}

trait UserService {
  this: Logger =>
  def getUser(id: String): Unit = {
    log(s"Getting user with id $id
    
  }
}
```

### Abstract Classes and Traits:

Abstract classes and traits allow you to define common behavior that can be shared among multiple classes.

```scala
trait Animal {
  def sound(): Unit
}

class Dog extends Animal {
  def sound(): Unit = println("Woof!")
}
```

### Implicit Classes:

Implicit classes allow you to add new methods to existing classes without modifying their code.

```scala
implicit class RichString(str: String) {
  def customMethod(): String = str.reverse
}

val reversed = "Scala".customMethod()  // Implicit conversion happens automatically
```

### Type Classes:

Type classes provide a way to achieve polymorphism without inheritance. It's a pattern used in functional programming.

```scala
trait Serializer[A] {
  def serialize(value: A): String
}

case class Person(name: String, age: Int)

implicit object PersonSerializer extends Serializer[Person] {
  def serialize(person: Person): String = s"${person.name}, ${person.age} years old"
}

def toJson[A](value: A)(implicit serializer: Serializer[A]): String = serializer.serialize(value)

val personJson = toJson(Person("John", 25))
```

## 44. Inheritance

Inheritance in Scala is similar to other object-oriented languages like Java, but Scala provides some additional features and flexibility.

```scala
// Define a base class
class Animal(var name: String) {
  def sound(): String = "Some generic sound"
}

// Create a subclass (inherits from Animal)
class Dog(name: String, breed: String) extends Animal(name) {
  override def sound(): String = "Woof"
  
  def fetch(): String = s"$name is fetching"
}

// Create another subclass (inherits from Animal)
class Cat(name: String, color: String) extends Animal(name) {
  override def sound(): String = "Meow"
  
  def climb(): String = s"$name is climbing"
}

// Create instances of the subclasses
val myDog = new Dog("Buddy", "Labrador")
val myCat = new Cat("Whiskers", "Gray")

// Access methods from the base class and subclasses
println(myDog.name)        // Output: Buddy
println(myDog.sound())     // Output: Woof
println(myDog.fetch())     // Output: Buddy is fetching

println(myCat.name)        // Output: Whiskers
println(myCat.sound())     // Output: Meow
println(myCat.climb())     // Output: Whiskers is climbing
```

In this example:

Animal is the base class with a property name and a method sound.

Dog and Cat are subclasses that extend Animal. They inherit the name property and override the sound method with their specific implementation.

Dog has an additional method fetch, and Cat has an additional method climb.

Instances of Dog and Cat can access both the inherited methods from Animal and their own specific methods.

The use of override keyword is important when you want to provide a specific implementation for a method in the subclass.

Scala also supports abstract classes and traits, which provide more flexibility in designing class hierarchies. 

Abstract classes can have abstract methods (methods without implementation), and traits are similar to Java interfaces.

## 45. Traits Part 1

In Scala, traits are similar to **interfaces** in other languages, but they can also contain concrete implementations.

They allow you to encapsulate method and field definitions, which can then be mixed into classes.

```scala
// Define a trait
trait Greetable {
  def greet(): Unit = {
    println("Hello, I can greet!")
  }
}

// Use the trait in a class
class Person(val name: String) extends Greetable

// Create an instance of the class
val person = new Person("Alice")

// Call the method from the trait
person.greet()
```

In this example, we've defined a trait Greetable with a method greet.

The Person class extends the Greetable trait, so it inherits the greet method. When we create an instance of Person and call the greet method, it prints "Hello, I can greet!".

Traits can also require that the classes mixing them in provide specific implementations. Here's an example:

```scala
trait Speaker {
  def speak(): Unit // Abstract method
}

class EnglishSpeaker extends Speaker {
  def speak(): Unit = {
    println("Hello, I speak English!")
  }
}

class FrenchSpeaker extends Speaker {
  def speak(): Unit = {
    println("Bonjour, je parle français!")
  }
}
```

In this case, the Speaker trait has an abstract method speak, and both EnglishSpeaker and FrenchSpeaker classes provide concrete implementations. 

When you create instances of these classes and call the speak method, you get language-specific greetings.

These are just basic examples, and traits can be much more powerful, especially when combined with other Scala features like mixin composition and self-types. 

They provide a flexible way to compose behavior in Scala classes.

## More traits examples:

### Stackable Traits:

```scala
// Stackable traits for modifying behavior
trait Doubling extends IntQueue {
  abstract override def put(x: Int): Unit = {
    super.put(2 * x)
  }
}

trait Incrementing extends IntQueue {
  abstract override def put(x: Int): Unit = {
    super.put(x + 1)
  }
}

// Base trait
abstract class IntQueue {
  def get(): Int
  def put(x: Int): Unit
}

// Concrete class mixing in the traits
class BasicIntQueue extends IntQueue {
  private var queue = List[Int]()

  def get(): Int = queue.head
  def put(x: Int): Unit = {
    queue = queue :+ x
  }
}

// Using the traits
val queue = new BasicIntQueue with Doubling with Incrementing
queue.put(1)
println(queue.get()) // Output: 4 (doubled and incremented)
```

In this example, Doubling and Incrementing are stackable traits that modify the behavior of the put method in IntQueue. 

The BasicIntQueue class mixes in these traits, creating a new class with the combined behavior.

### Self-types:

```scala
// Self-type for enforcing dependencies
trait Logging {
  def log(message: String): Unit
}

trait UserService {
  this: Logging =>

  def getUser(id: String): String = {
    log(s"Fetching user with id $id")
    // Logic to fetch user
    s"User #$id"
  }
}

// Using the traits
val userService = new UserService with Logging {
  def log(message: String): Unit = {
    println(s"Log: $message")
  }
}

println(userService.getUser("123")) // Output: User #123 with logging
```

In this example, the UserService trait has a self-type this: Logging =>, which means any class or trait that mixes in UserService must also mix in Logging.

This enforces a dependency relationship.

### Abstract and Concrete Fields:

```scala
// Abstract and concrete fields in a trait
trait Animal {
  val species: String
  var age: Int

  def makeSound(): Unit
}

class Dog extends Animal {
  val species: String = "Canine"
  var age: Int = 3

  def makeSound(): Unit = {
    println("Woof!")
  }
}

// Using the trait
val dog = new Dog
println(s"Species: ${dog.species}, Age: ${dog.age}")
dog.makeSound()
```

In this example, the Animal trait has an abstract field species and a concrete field age.

The Dog class extends Animal and provides concrete implementations for these fields.

These examples showcase some of the versatility of traits in Scala, from modifying behavior to enforcing dependencies and providing abstract or concrete fields.

## 46. Traits Part 2



## 47. Multiple Traits



## 48. Access modifiers: private, public, protected.



## 49. Constructors




## 50. Auxiliary constructors




## 51. Multiple constructors




## 52. Singleton Objects




## 53. Companion Objects




## 54. Create instances with new




## 55. Case class




## 56. Abstract class





# Functional programming

Functional programming (FP) is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids changing state and mutable data. 

Scala is a versatile programming language that supports both object-oriented and functional programming.

### Immutable Data:

In functional programming, data is immutable, meaning once it's defined, it cannot be changed. 

In Scala, you often use the **val** keyword for immutable values.

```scala
val x = 5
// x = 7  // This would result in a compilation error
```

### First-Class Functions:

Functions are first-class citizens, which means you can pass functions as arguments to other functions, return functions from functions, and assign functions to variables.

```scala
def add(x: Int, y: Int): Int = x + y

val sum = add(3, 4)
println(sum)  // Output: 7
```

### Higher-Order Functions:

Higher-order functions take one or more functions as arguments or return a function.

map, filter, and reduce are commonly used higher-order functions.

```scala
val numbers = List(1, 2, 3, 4, 5)

val squared = numbers.map(x => x * x)
// squared: List[Int] = List(1, 4, 9, 16, 25)

val evens = numbers.filter(x => x % 2 == 0)
// evens: List[Int] = List(2, 4)

val sum = numbers.reduce((x, y) => x + y)
// sum: Int = 15
```

### Pattern Matching:

Pattern matching is a powerful feature in functional programming languages. 

It allows you to match values against patterns and execute code based on the matched pattern.

```scala
def describe(x: Any): String = x match {
  case 0 => "Zero"
  case n if n > 0 => "Positive number"
  case n if n < 0 => "Negative number"
  case _ => "Other"
}

println(describe(5))  // Output: Positive number
```

### Recursion:

Instead of using loops, functional programming often relies on recursion for repetitive tasks.

```scala
def factorial(n: Int): Int =
  if (n <= 1) 1
  else n * factorial(n - 1)

println(factorial(5))  // Output: 120
```

These are just a few concepts and examples of functional programming in Scala.

FP can lead to more concise, readable, and maintainable code by avoiding mutable state and side effects.

## 57. High Order Functions

In Scala, high-order functions are functions that take other functions as parameters or return functions. 

They are a powerful concept in functional programming. Let me give you some examples:

### Function as a Parameter:

```scala
// A high-order function that takes a function as a parameter
def operateOnNumbers(a: Int, b: Int, operation: (Int, Int) => Int): Int = {
  operation(a, b)
}

// Define a function to add two numbers
val add: (Int, Int) => Int = (x, y) => x + y

// Use the high-order function with the add function
val result = operateOnNumbers(3, 5, add)
println(result) // Output: 8
```

Here, operateOnNumbers is a high-order function that takes two numbers and a function (operation).

You can pass different functions as the third parameter, like add in the example.

### Function as a Return Type:

```scala
// A high-order function that returns a function
def multiplier(factor: Int): Int => Int = {
  (x: Int) => x * factor
}

// Use the high-order function to create a specific multiplier
val multiplyBy3 = multiplier(3)

// Now, use the returned function
val result = multiplyBy3(4)
println(result) // Output: 12
```

In this example, multiplier is a high-order function that takes an Int and returns a function (Int => Int). 

The returned function (multiplyBy3) can then be used to multiply numbers by 3.

These examples showcase how high-order functions make code more flexible and expressive by allowing you to pass functions around as if they were data.

## More advanced concepts related to high-order functions in Scala:

### Function Composition:

High-order functions can be composed to create new functions. 

Scala provides the compose and andThen methods for function composition.

```scala
// Function composition using andThen
val add2: Int => Int = _ + 2
val multiplyBy3: Int => Int = _ * 3

val composedFunction: Int => Int = add2 andThen multiplyBy3

val result = composedFunction(5)
println(result) // Output: 21 (add 2, then multiply by 3)
```

Here, andThen creates a new function that first applies add2 and then applies multiplyBy3.

### Currying:

Currying is a technique where a function with multiple parameters is transformed into a series of functions, each taking a single parameter.

```scala
// Currying example
def addCurried(x: Int)(y: Int): Int = x + y

val add5: Int => Int = addCurried(5)

val result = add5(3)
println(result) // Output: 8
```

addCurried is a curried function. You can partially apply it, fixing the value of x and creating a new function (add5) that takes only y. This can be useful for creating specialized functions.

### Anonymous Functions (Lambda Expressions):

You can define anonymous functions (lambda expressions) directly where they are needed.

```scala
// Anonymous function example
val addOne: Int => Int = (x: Int) => x + 1

val result = addOne(7)
println(result) // Output: 8
```

Here, (x: Int) => x + 1 is an anonymous function assigned to addOne. It takes an integer x and adds 1 to it.

### Higher-Order Functions in Collections:

Many higher-order functions are available in Scala collections, such as map, filter, and reduce. 

They operate on elements of collections and take functions as parameters.

```scala
val numbers = List(1, 2, 3, 4, 5)

// Using map to double each element
val doubled = numbers.map(x => x * 2)

// Using filter to keep only even numbers
val evens = numbers.filter(_ % 2 == 0)

// Using reduce to find the sum
val sum = numbers.reduce(_ + _)
```

Here, map, filter, and reduce are higher-order functions that take functions as arguments to define their behavior.

These advanced topics demonstrate the flexibility and conciseness that high-order functions bring to Scala, enabling you to write more expressive and modular code.

## 58. Anonymous functions.

In Scala, anonymous functions are often referred to as "function literals" or "lambda expressions." 

They are a concise way to create functions without explicitly providing a name. 

The syntax for anonymous functions involves the => symbol.

```scala
// Define an anonymous function that takes two parameters and returns their sum
val add: (Int, Int) => Int = (x, y) => x + y

// Using the anonymous function
val result = add(3, 5)
println(result)  // Output: 8
```

In this example:

val add declares a value (immutable) named add.

(Int, Int) => Int specifies the types of parameters and the return type of the anonymous function.

(x, y) => x + y is the actual anonymous function, where x and y are the parameters, and x + y is the expression to be evaluated.

Here's another example using a higher-order function:

```scala
// Define a higher-order function that takes two integers and a function,
// and applies the function to the integers
def operateOnNumbers(x: Int, y: Int, operation: (Int, Int) => Int): Int = {
  operation(x, y)
}

// Using the higher-order function with an anonymous function
val result1 = operateOnNumbers(10, 5, (a, b) => a + b)
val result2 = operateOnNumbers(10, 5, (a, b) => a * b)

println(result1)  // Output: 15
println(result2)  // Output: 50
```

In this example, operateOnNumbers is a higher-order function that takes two numbers and a function as parameters.

It applies the provided function to the numbers.

Anonymous functions are particularly handy when you need a short, one-off function for a specific operation. 

They're concise and often used with higher-order functions like map, filter, and reduce in Scala.

## Functions literals

In Scala, function literals are anonymous functions that you can define on the fly. 

They are also known as anonymous functions or lambda functions. 

The syntax for function literals is concise and expressive.

Here's a simple explanation with examples:

Basic Syntax:

(parameters) => expression

### Example 1: Simple Addition

```scala
val add = (a: Int, b: Int) => a + b
println(add(2, 3)) // Output: 5
```

In this example, add is a function literal that takes two parameters a and b and returns their sum.

### Example 2: Multi-line Expression

```scala
val multiply = (a: Int, b: Int) => {
  val result = a * b
  result
}
println(multiply(2, 3)) // Output: 6
```

You can use curly braces for a multi-line expression. The last line of the block is the return value.

### Example 3: Function as a Parameter

```scala
def operate(x: Int, y: Int, operation: (Int, Int) => Int): Int = {
  operation(x, y)
}

val result = operate(3, 4, (a, b) => a * b)
println(result) // Output: 12
```

Here, the operate function takes two numbers and a function as parameters. The third parameter is a function literal for the operation.

Using Underscore _:

```scala
val square: Int => Int = _ * _
println(square(5)) // Output: 25
```

The underscore is a shorthand notation for parameters. In this example, _ * _ is a concise way to express a function that squares its input.

Function literals in Scala are powerful and provide a concise way to express functionality, especially when you need to pass functions as parameters or return them from other functions.

## 59. Functions with parameters



## 60. Functions as variables



## 61. Return a function



## 62. Partially Applied Functions



## 63. Currying Functions



## 64. Closures



## 65. Options



## 66. Exceptions. Try Catch



## 67. Exceptions, finally



## 68. Exceptions, Throw



## 69. Overloading



## 70. Text files

In Scala, working with text files involves reading from and writing to files. 

Scala provides several ways to perform these operations. 

### Reading from a Text File

You can use the Source class in the scala.io package to read from a text file. Here's a simple example:

```scala
import scala.io.Source

// Specify the path to your text file
val filePath = "path/to/your/file.txt"

// Try to open the file and read its contents
try {
  val source = Source.fromFile(filePath)
  val lines = source.getLines().toList

  // Do something with the lines (e.g., print them)
  lines.foreach(println)

  // Close the source to release resources
  source.close()
} catch {
  case e: Exception => println(s"An error occurred: ${e.getMessage}")
}
```

### Writing to a Text File

To write to a text file, you can use java.io.PrintWriter or other similar classes. Here's an example:

```scala
import java.io.PrintWriter

// Specify the path to your output file
val outputPath = "path/to/your/output.txt"

// Try to open the file for writing
try {
  val writer = new PrintWriter(outputPath)

  // Write some lines to the file
  writer.println("Hello, Scala!")
  writer.println("This is a sample text file.")
  writer.println("Writing to files in Scala is fun!")

  // Close the writer to flush and release resources
  writer.close()

  println("Write operation successful.")
} catch {
  case e: Exception => println(s"An error occurred: ${e.getMessage}")
}
```

Creating and deleting text files in Scala involves using Java's File class. Here are examples for both operations:

### Creating a Text File

```scala
import java.io.PrintWriter

// Specify the path for the new file
val filePath = "path/to/your/newfile.txt"

// Try to create the file
try {
  val writer = new PrintWriter(filePath)

  // Write some content to the file
  writer.println("This is a new text file created in Scala.")
  writer.println("You can add more content here.")

  // Close the writer to flush and release resources
  writer.close()

  println(s"File created successfully at: $filePath")
} catch {
  case e: Exception => println(s"An error occurred: ${e.getMessage}")
}
```

### Deleting a Text File

```scala
import java.io.File

// Specify the path to the file to be deleted
val filePathToDelete = "path/to/your/file-to-delete.txt"

// Create a File object
val fileToDelete = new File(filePathToDelete)

// Try to delete the file
try {
  if (fileToDelete.delete()) {
    println(s"File deleted successfully: $filePathToDelete")
  } else {
    println(s"Unable to delete the file: $filePathToDelete")
  }
} catch {
  case e: Exception => println(s"An error occurred: ${e.getMessage}")
}
```

Make sure to replace the file paths with the actual paths you want to use. Also, handle exceptions appropriately in your actual code for robust error management.

Let's delve into more advanced topics related to working with text files in Scala. We'll cover concepts such as reading and writing CSV files, working with larger files, and using more advanced libraries.

### 1. Reading and Writing CSV Files

Working with CSV (Comma-Separated Values) files is a common task. 

You can use libraries like opencsv or built-in functions in Scala for this.

Using OpenCSV Library:

Add the following dependency to your project:

```scala
libraryDependencies += "com.opencsv" % "opencsv" % "5.6"
```

Now you can use OpenCSV for CSV operations:

```scala
Copy code
import au.com.bytecode.opencsv.CSVReader
import au.com.bytecode.opencsv.CSVWriter

// Reading from CSV
val reader = new CSVReader(new FileReader("path/to/your/input.csv"))
val lines: List[Array[String]] = reader.readAll()

// Writing to CSV
val writer = new CSVWriter(new FileWriter("path/to/your/output.csv"))
val data = Array("Column1", "Column2", "Column3")
writer.writeNext(data)
writer.close()
```

### 2. Working with Large Files

For large files, you may want to consider streaming instead of loading the entire file into memory.

Scala's scala.io.Source can help with this.

```scala
import scala.io.Source

val filePath = "path/to/largefile.txt"

// Use Source to stream lines without loading the entire file into memory
val source = Source.fromFile(filePath)
try {
  source.getLines().foreach { line =>
    // Process each line as needed
    println(line)
  }
} finally {
  source.close()
}
```

### 3. Using java.nio.file for File Operations

The java.nio.file package provides a more modern and flexible API for file operations.

```scala
import java.nio.file.{Paths, StandardCopyOption, Files}

val sourcePath = Paths.get("path/to/source.txt")
val destinationPath = Paths.get("path/to/destination.txt")

// Use Files.copy for file copy operations
Files.copy(sourcePath, destinationPath, StandardCopyOption.REPLACE_EXISTING)
```

### 4. Using Apache Commons IO Library

Apache Commons IO is a powerful library that simplifies many common I/O operations. To use it, add the following dependency:

```scala
libraryDependencies += "commons-io" % "commons-io" % "2.11.0"
```

Now you can use it for various file-related operations:

```scala
import org.apache.commons.io.FileUtils

val sourceFile = new File("path/to/source.txt")
val destinationFile = new File("path/to/destination.txt")

// Copying a file
FileUtils.copyFile(sourceFile, destinationFile)

// Deleting a directory
FileUtils.deleteDirectory(new File("path/to/directory"))
```



## 71. Binary files

Reading and writing binary files in Scala involves using input and output streams to handle the raw binary data. Let me provide you with some simple examples.

### Reading Binary File:

```scala
import java.io.{File, FileInputStream, DataInputStream}

// Specify the path to your binary file
val filePath = "path/to/your/file.bin"

// Create a FileInputStream for the binary file
val fileInputStream = new FileInputStream(new File(filePath))

// Wrap the FileInputStream with a DataInputStream for convenient methods
val dataInputStream = new DataInputStream(fileInputStream)

try {
  // Read bytes from the binary file
  val byteArray = new Array[Byte](fileInputStream.available())
  dataInputStream.readFully(byteArray)

  // Process the binary data as needed
  // ...

} finally {
  // Close the streams to release resources
  dataInputStream.close()
  fileInputStream.close()
}
````

### Writing Binary File:

```scala
import java.io.{File, FileOutputStream, DataOutputStream}

// Specify the path for the new binary file
val filePath = "path/to/new/file.bin"

// Create a FileOutputStream for the new binary file
val fileOutputStream = new FileOutputStream(new File(filePath))

// Wrap the FileOutputStream with a DataOutputStream for convenient methods
val dataOutputStream = new DataOutputStream(fileOutputStream)

try {
  // Create a sample byte array to write to the binary file
  val byteArray = Array[Byte](0x48, 0x65, 0x6C, 0x6C, 0x6F) // "Hello" in ASCII

  // Write the byte array to the binary file
  dataOutputStream.write(byteArray)

  // Optionally, write more data
  // ...

} finally {
  // Close the streams to release resources
  dataOutputStream.close()
  fileOutputStream.close()
}
```

In these examples, DataInputStream and DataOutputStream provide convenient methods for reading and writing various primitive data types.

Adjust the code as needed based on the specific format and structure of your binary file. 

Keep in mind that error handling, such as using try-with-resources, is crucial to ensure proper resource management.

Creating and deleting a binary file in Scala involves using the java.nio.file package. Here's a simple example:

### Creating a Binary File:

```scala
import java.nio.file.{Files, Paths, StandardOpenOption}
import java.nio.ByteBuffer

// Specify the path for the new binary file
val filePath = "path/to/new/file.bin"

// Sample data to write to the binary file
val data = Array[Byte](0x48, 0x65, 0x6C, 0x6C, 0x6F) // "Hello" in ASCII

// Use ByteBuffer to write binary data
val buffer = ByteBuffer.wrap(data)

// Create the binary file
Files.write(Paths.get(filePath), buffer.array(), StandardOpenOption.CREATE)
```

### Deleting a Binary File:

```scala
import java.nio.file.{Files, Paths}

// Specify the path of the binary file to delete
val filePathToDelete = "path/to/new/file.bin"

// Delete the binary file
Files.deleteIfExists(Paths.get(filePathToDelete))
```

In the creation example, we use Files.write to write the binary data to the specified file path. We use ByteBuffer to wrap the byte array for convenient writing.

Adjust the StandardOpenOption based on your requirements (e.g., StandardOpenOption.CREATE_NEW to create a new file only if it does not exist).

In the deletion example, we use Files.deleteIfExists to delete the file at the specified path.

It ensures that the file is deleted if it exists, and it won't throw an exception if the file doesn't exist.

Make sure to handle exceptions appropriately in your actual code to account for cases where file operations might fail, especially when dealing with file I/O.

## More advanced topics about binary files in Scala

### 1. Random Access Files:

You can use RandomAccessFile for more advanced scenarios where you need to perform random access reads and writes at specific positions within the file. 

This can be useful for large files or when you need to update specific portions of the file without reading and rewriting the entire content.

```scala
import java.io.RandomAccessFile

val filePath = "path/to/your/file.bin"

val randomAccessFile = new RandomAccessFile(filePath, "rw")

try {
  // Move the file pointer to a specific position
  randomAccessFile.seek(10)

  // Read or write data at the current file pointer position
  // ...

} finally {
  randomAccessFile.close()
}
```

### 2. Memory-Mapped Files:

Memory-mapped files provide a way to map a region of a file directly into memory. 

This can be more efficient for certain types of file access, especially for large files. 

Scala supports memory-mapped files through the java.nio.channels.FileChannel class.

```scala
import java.nio.channels.{FileChannel, FileChannel.MapMode}
import java.nio.file.{Paths, StandardOpenOption}

val filePath = "path/to/your/largefile.bin"

val fileChannel = FileChannel.open(Paths.get(filePath), StandardOpenOption.READ)

try {
  // Map the entire file into memory
  val mappedByteBuffer = fileChannel.map(MapMode.READ_ONLY, 0, fileChannel.size())

  // Access the data through the ByteBuffer
  // ...

} finally {
  fileChannel.close()
}
```

### 3. Handling Different Data Types:

When working with binary files, you often encounter different data types (e.g., integers, floating-point numbers). 

You can use classes like java.nio.ByteBuffer to convert between binary data and various data types.

```scala
import java.nio.ByteBuffer

val intData = 42

// Convert integer to bytes
val intBytes = ByteBuffer.allocate(4).putInt(intData).array()

// Convert bytes back to integer
val retrievedInt = ByteBuffer.wrap(intBytes).getInt()
```

#### 4. Bit-Level Manipulation:

For fine-grained control over binary data, you might need to perform bit-level manipulation. 

Scala provides bitwise operators (&, |, ^, <<, >>, >>>) for this purpose.

```scala
// Set the third bit to 1
val originalValue = 0b00000100
val modifiedValue = originalValue | (1 << 2)
```

These advanced topics give you more tools for efficiently working with binary files in Scala, depending on the specific requirements of your application.

Always remember to handle exceptions and resource cleanup appropriately to ensure robust file handling.
