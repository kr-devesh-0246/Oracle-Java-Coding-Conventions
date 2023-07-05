# Blank Lines 
Blank lines improve readability by setting off sections of code that are logically related. 

Two blank lines should always be used in the following circumstances:
- Between sections of a source file
- Between class and interface definitions

One blank line should be used in the following circumstances:
- Between methods
- Between the local variables in a method and its first statement
- Before a block or single-line comment
- Between logical sections to improve readability

# Blank Spaces
Blank spaces should be used in the following circumstances:
- A keyword followed by a parenthesis should be separated by a space. 
```java
while (true) {
    ...
}
```
**Note**: A blank space should not be between a *method name* and its *opening parenthesis*. This helps to distinguish keywords from method calls.

- A blank space should appear after commas in argument list.
- All binary operators except . should be seperated from their operands by spaces. 
- A blank spaces should never separate unary operators such as unary minus, increment("++"), and decrement("--") from their operands. 
**Example**
```java
a += c + d;
a = (a + b) / (c * d);

while (d++ = s++) {
    n++;
}
printf("size is " + foo + "\n");
```

- The expression in a for statement should be separated by blank spaces. 
Example
```java
for (exp1; exp2; exp3)
```

Casts should be followed by a blank. 
```java
myMethod((byte) aNum, (Object) x);
myFunc((int) (cp + 5), ((int) (i + 3)) + 1);
```
