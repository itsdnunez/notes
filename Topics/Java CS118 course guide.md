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

;;;;;;;;;; page 32, 4.3


## Iteration

### While loops

### For loops 

## Input and Ouput

3 I/O streams, 2 for output (output stream and error stream) 

> System.out, System.err and System.in

Use PrintStrem documentation for methods

#### Scanners

For input streams, read byte-by-byte or use another class - Java provides Scanner for this

Scanners are declared:
```java
Scanner sc = new Scanner(System.in);
long aLong = sc.nextLong();
double aDouble = sc.nextDouble();
```

####  Exercise


## Methods

## OOP

## Debugging 



