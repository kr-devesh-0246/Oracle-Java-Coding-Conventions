# Code Examples

## Java Source File Example
The following example shows how to format a Java source file containing a single public class. Interface are formatted similarly.
```java
/*
* %W% %E% Firstname Lastname
*
* Copyright (c) 1993-1996 Sun Microsystems, Inc. All Rights Reserved.
*
* This software is the confidential and proprietary information of Sun
* Microsystems, Inc. ("Confidential Information"). You shall not
* disclose such Confidential Information and shall use it only in
* accordance with the terms of the license agreement you entered into
* with Sun.
*
* SUN MAKES NO REPRESENTATIONS OR WARRANTIES ABOUT THE SUITABILITY OF
* THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
* TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
* PARTICULAR PURPOSE, OR NON-INFRINGEMENT. SUN SHALL NOT BE LIABLE FOR
* ANY DAMAGES SUFFERED BY LICENSEE AS A RESULT OF USING, MODIFYING OR
* DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
*/
package java.blah;
import java.blah.blahdy.BlahBlah;
/**
* Class description goes here.
*
* @version
1.10 04 Oct 1996
* @author
Firstname Lastname
*/
public class Blah extends SomeClass {
/* A class implementation comment can go here. */
/** classVar1 documentation comment */
public static int classVar1;
/**
* classVar2 documentation comment that happens to be
* more than one line long
*/
private static Object classVar2;
/** instanceVar1 documentation comment */
public Object instanceVar1;
/** instanceVar2 documentation comment */
protected int instanceVar2;
/** instanceVar3 documentation comment */
private Object[] instanceVar3;
/**
* ...method Blah documentation comment...
*/
public Blah() {
// ...implementation goes here...
}
/**
* ...method doSomething documentation comment...
*/
public void doSomething() {
// ...implementation goes here...
}
/**
* ...method doSomethingElse documentation comment...
* @param someParam description
*/
public void doSomethingElse(Object someParam) {
// ...implementation goes here...
}
}
```