# Java Notes

## Syllabus:
- Intro to OOP and Java
- Values and Data Type
- Operators in java
- Input in Java
- Mathematical Library Methods
- Conditional Statements in Java
- Iterative Constructs in Java
- Nested for Loops
- Basic Input Output (Scanner and Printer Classes)*

## Intro to OOP and Java
An Object Oriented Programming tries to make real world things as code, short and easy to understand.
OOP Focuses on code reusability.

### Class
Blueprint for creating object.

### Object
Instance of a Class.

### Few Terms used 
- Class -> Student
- Attributes -> name, class, rollno
- Methods -> get_result(), attendence()

### Few Important Concepts
- Abstraction -> Hiding Internal Details. example: a phone
- Encapsulation -> Putting various components together. (Sesitive data can be hidden from the users) example: Laptop
- Inheritance -> New thing from Existing thing example: Bun-Tikki from Bun
- Polymorphism -> One Thing can do more stuff. example : Smartphone as phone also as a calculator or as a camera.

## Values and Data Types
Data Types specify the different sizes and values that can be stored in the variable.
There are two types of Data Types in Java:
- Primitive Data Types : boolean, char, byte, short, int, long, float, double.
- Non-Primitive Data Types: Classes, Arrays, Strings.

boolean -> true false
byte, short, int, long -> integers
float, double -> real numbers (decimal point ones)

## Operators in Java
Operators in Java are mostly like that in Mathematics.
They are used to perform operations on variables and values.
1(operand) +(operator) 3(operand) = 4(Result)

### Types of Operators
- Arithmatic Operators -> +, -, *, /, % ....
- Assignment Operators -> =, +=, -=, *=, /= ...
- Comparison Operators -> ==, >=, <=
- Logical Operators -> &&, ||, !
- Bitwise operators -> &, |

Study the Precedence of Operators (Impt. for School Exams)

Associativity tells the direction of execution of operators It can either be left to right or right to left.
*, / -> Left to Right
+, - -> Left to Right
++, = -> Right to Left
### Resulting Data Types
Look at the Following Table:

| Type1      | Type2     | ResultTypes |
|------------|-----------|-------------|
| Boolean    | short     | int         |
| short      | int       | int         |
| long       | float     | float       |
| int        | float     | float       |
| char       | int       | int         |
| char       | short     | int         |
| long       | double    | double      |
| float      | double    | double      |

### Increment and Decrement Operators
a++, ++a -> Increment Operators
a--, --a -> Decrement Operators
Can be used with any datatypes
a++ -> first use the value then increment
++a -> first increment then use it

## Input in Java

```java
import java.util.*;
class InputDemo
{
public static void main(String[] args)
{
Scanner sc= new Scanner(System.in); // System call input stream
System.out.println("Enter First Number: ");
int a = sc.nextInt();
System.out.println("Now Enter a Float Number: ");
float b = sc.nextFloat();
System.out.println("User Input One "+a+" User Input Two "+b);
}
}
```

## Mathematical Library Methods
NO need to import we can just use the Methods.
A Few Methods available: min(), max(), avg(), sin(), cos(), tan(), round(),ceil(), floor(), abs() etc.

```java
import java.util.*;
class MathExample
{
public static void main(String[] args)
{
Scanner sc = new Scanner(System.in)
System.out.println("Enter Number You want root of: ");
int a = sc.nextInt();
float root=Math.sqrt(a);
System.out.println("Square Root of "+a+" = "+root);
}
}
```

## Conditional Statements in Java
if-else and switch
Conditional Statements can be nested.

```java
// We can use standalone if statement
if(a==b){
something that happens in this case;
}
// else has to be used with an if statement
else{
what to else
}
```
```java
switch(value){
case x:
		somethings happen
		break;
case y:
		something happen
		break;
default:
		something default you want to happen
}
```

## Iterative Constructs in Java
Iterative Constructs basically means Loops.
Java has 3 types of Loops:
- while
- do-while
- for

while loop is used when we are uncertain of the number of times we have to loop.

### while and do-while
while loop checks the condition first before execution.
do-while loop executes at least once, if the condition is false.

```java
// while loop example
int a= 1;
while(a<11){
System.out.println(a);
a=a+1 // a++ same stuff
}
// do-while loop example
do{
System.out.println(a)
a++
}while(a<11);
```

### for loop
for loop is more like as it also checks the condition before execution.
```java
for(int a=0;a<11;a++)
{
System.out.println(a);
}
```
## Nested for Loops
In Java like in most programming languages we can nest stuff.
Nesting a for loop means using a for inside other for loop.
This is what is used to create those Pattern Programs.

```java
for(int i=1;i<11;i++){
System.out.println("Table of "+i);
for(int j=1;j<11;j++){
System.out.println(i+" X "+j+" = "+(i*j));
}
}
```

## Buffered Reader

```java
import java.io.*;
public class BuffReader
{
public static void main(String[] args)throws Exception
{
InputStreamReader r=new InputStreamReader(System.in);
BufferedReader br=new BufferedReader(r);
System.out.println("Enter a Number ");
int num=Integer.parseInt((br.readLine()));
System.out.println("Your Number is "+num);
br.close();
r.close();
}
}
```








