# File Organization

A file consists of sections that should be seperated by blank lines and an optional* comment identifying each section.

Files longer than 2000 lines are cumbersome and should be avoided.

## Java Source Files

- Each java source file contains a single public class or interface. And it should be the first class or interface in the file.

- When private classes and interfaces are associated with a public class, you can put them in the same source file as the public class.

**Java sourse files have the following ordering:**

- Beginning comments
- Package and Import statements
- Class and interface declarations(see in below tables) 

### Beginning Comments
All source files should begin with a c-style comment that lists the programmer(s), the date, a copyright notice, and also a brief description of the purpose of the program. 

*For example*
```java
/**
  * Classname
  * Version info
  * Copyright notice
  */
```
### Package and Import Statements
The first non-comment line of most Java source files is a package statement. 

After that, import statements can follow. 

*For example*
```java
package com.devesh;

import java.util.*;
```

### Class and Interface Declarations

The following table describes the parts of a class or interface declaration, in the order that they should appear. 

| | Part of Class/Interface|Notes|
|---|---|---|
|1 | Class/interface documentation comment|See "documentation comments"|
|2|class or interface statement||
|3|Class/interface implementation comment(```/*...*/```), if necessary|This comment should contain any class-wide or interface-wide information that wasn't appropriate for the class/interface documentation comment.|
|4|Class (Static) variables|First public, then protected, and then private.||
|5|Instance variables|First public, then protected, and then private.|
|6|Constructors||
|7|Methods|These methods should be grouped by functionality rather than by scope or accessibility(i.e. access specifier based). |