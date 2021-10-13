# Welcome 

- So basically remember to put .java in filenames
- Also name your classes the same as the filename

## Starting files

```java
public class MyClass {
    public static void main(String[] args) {
      //p    
    }
}
```

## Variables

Do not use ($) or start variable name with an (_) 

#### Variable scope

- Where a variable is declared, it only exists within the curly braces
- Variables declared outside of methods are instance/ class variables - they maintain values between functions
- 2 variables with the same names may be able to coexist given their scopes do not overlap

#### Types of variable:
- byte - -2^7 to 2^7-1
- short - 2^15
- int - 2^31
- long - 2^63
- float - 32-bit floating point, roughly 6 digits of precision
- double - 64-bit floating point, roughly 15 digits of precision
- char - 16-bit type representing any character in UTF-16 set
- boolean - T/F

#### Bonus Memes 
 
Declared values are *int* by default so do (Number)L for large numbers

## Objects

Names start with capital letters 

#### String operator 

s.charAt(n); // where n is the position of the chosen character

## Arrays

Store collections of similar objects

#### Declaration

Declaring the array requires 

> type arrayName[] = new type[arrayLength]

Declaring values in the array 

> arrayName[place in array] = x;

## Conditional Statements

### If statements

```java
if (condition) {
} elseif (condition) {
} else {
]
```

can also use &&, or || - a single one is strict, double is lazy

### Switch statements

- If you want to evaluate multiple cases, but if a break is encoutnered, Java skips to the end of the break switch statement
- If no cases are matched, default case will be executed unless it is absent
```java
switch (variable) {
    case 1:...
        break;
    case 2:...
        ...
    default: ...      
}
```

## Iteration

### While 

```java
while (condition){
    //code
}
```

When code needs to be evaluated after the body has been executed use

```java
do {
    //code
} while (condition);
```

### For loops 

Formatting for loops

```java
for (initial condition; termination condition; iteration operation){
    //code 
}
```

## Input and Ouput

3 I/O streams, 2 for output (output stream and error stream) 

> System.out, System.err and System.in

Use PrintStrem documentation for methods

#### Scanners

**Import Scanner**

For input streams, read byte-by-byte or use another class - Java provides Scanner for this

Scanners are declared:
```java
Scanner sc = new Scanner(System.in);
long aLong = sc.nextLong();
double aDouble = sc.nextDouble();
```

## Methods

- Allow repeated subproblems to reuse the same code = less code and facilitates changes and extensions 
- All methods have names - list of parameters and a return type

> when no return type use 'void'

```java
[access][type] methodName([returnType] parameterName, [type] parameterName,...){
...
}
```

#### Access types

Methods can be public, private or protected

## OOP

- Almost everything is an object - instance of a class initialised with the *new* keyword 
- Access modifiers allow *encapsulation* - generally use private variables and public methods in object oriented code
- Class variables must be private - can only be changed by method in the class
- Safest way to program - make all things private unless external access is required

#### Inheritance

- Classes can be created that inherit properties and mehtods from other classes
> [type] class [newObject] extends [className]{
> }

These extended classes can be further extended with their own properties

## Debugging 

- Syntatic error - occurs at compile time 
- Semantic error - code understood by compiler but logic is incorrect 





