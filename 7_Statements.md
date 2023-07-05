# Statements
## 1. Simple Statements
Each line should contain at most one statement. 
```java
arg_v++; arg_c--; // AVOID!
```
Do not use the comma operator to group multiple statements unless it is for an obvious reason. 
```java
if(err) {
    Format.print(System.out, "error"), exit(1); // VERY WRONG!
}
```
## 2. Compound Statements
Compound statements contain lists of statements enclosed in braces "{statements}". 
- The enclosed statements should be indented one more level than the compund statement. 
- The opening brace should be at the end of the line that begins the compound statement. 
- Braces are used around all statements, even singletons, when they are part of the control structure. This makes it easier to add statements without accidently introducing bugs due to forgetting to add braces. 

## 3. return Statements
A return statement with a value should not use parenthesis unless they make the return value more obvious in some way. 
```java
return;
return flag;
return (size ? size : defaultSize); 
```

## 4. if, if-else, if-else-if-else Statements
The if-else class of statements should have the following form:
```java 
// only if
if (condition) {
    statements;
}

// if-else
if (condition) {
    statements;
} else {
    statements;
}

//if-else-if-else
if (condition) {
    statements;
} else if (condition) {
    statements;
}
```

**Note**
if statement always use braces {}. Avoid the following error-prone form:
```java
if(condition) //AVOID!   
    statement;
```

## 5 for Statements
A for statement should have the following form:
```java
for (initialization; condition; update) {
    statements;
}
```
An empty for statement should be avoided.
```java
for (initialization; condition; update); // All the work is done in the for loop parameter
```
- When using the comma operator in the initialization or update clause of a for statement, avoid teh complexity of using more than three variables. 

- If needed, use separate statements before the for loop (for the initialization clause) or at the end of the loop (for the update clause).

## 6 while Statements
A while statement should have the following form: 
```java
while (condition) {
    statements;
}
```

An empty while statement should have the following form:
```java
while (condition);
```

## 7 do-while Statements
A do-while statement should have the following form:
```java
do {
    statements;
}
while (condition) ;
```

## 8 switch Statements
A switch statement should have the following form:
```java
switch (condition) {
case ABC:
    statements;
    /*falls through*/
case DEF:
    statements;
    break;
case XYZ:
    statements;
    break;
default:
    statements;
    break;    
}
```
Every time a case falls through(doesn't include a break statement), statement would normally be. This is shown in the preceding code example with the /* falls through */ comment.

Every switch statement should include a default case. This break is the default case is redundant, but it prevents a fall-through error if later another case is added. 

## 9 try-catch Statements
A try-catch statement should have teh following format:
```java
try{
    statements;
} catch (ExceptionClass e) {
    statements;
}
```


