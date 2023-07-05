# Declarations

## Number Per Line
One declaration per line is recommended since it encourages commenting. In other words, 
```java
int level; // indentation level
int size;  //size of table
```
is preferred over 
```java
int level, size;
```
In absolutely no case should variables and functions be declared on the same line. 

Example
```java
long phoneNumber, getPhoneNumber(); // VERY WRONG!
```
Do not put different types on the same line. 

Example 
```java
int foo, fooarray[]; // WRONG!
```

**Note:** The examples above uses one spaces between the type and the same line. 

```java 
int level; // indentation level
int size;  // size of table
Object currentEntry; // currently selected table entry 
```

## Placement
Put declarations only at the beginning of the blocks. Don't wait to declare variables until their first use; it can confuse the unwary programmer and hamper code portability within the scope. 

```java
void myMethod() {
    int int1;         // beginning of method block 

    if (condition) {
        int int2;     // beginning of "if" block 
        ...
    }
}
```

The one exception to the rule is indexes of for loops, at higher levels, which in Java can be declared in the for statement:
```java 
for (int i = 0; i < maxLoops; i++) {
    ...
}
```

Avoid local declarations that hide declarations at higher levels. For example, do not declare the same variable name in an inner block:
```java
int count;
...
func() {
    if (condition) {
        int count; // AVOID!
        ...
    }
    ...
}
```

## Initialization
Try to initialize local variables where they're declared. The only reason not to initialize a variable where it's declared is if intial value depends on some computation occuring first.

## Class and Interface Declarations
When coding Java classes and interfaces, the following formatting rules should be followed:
- No space between a method name and the parenthesis "("j starting its parameter list
- Open brace "{" appears at the end of the same line as the declaration statement
- Closing brace "}" starts a line by itself indented to match its corresponding opening statement, except when it is a null statement the "}" should appear immediately after the "{"
```java
class Sample extends Object {
    int ivar1;
    int ivar2;

    Sample(int i, int j) {
        ivar1 = i;
        ivar2 = j;
    }

    int emptyMethod() {} // HAVE A LOOK!
    ... 
}
```
- Methods are separated by a blank line