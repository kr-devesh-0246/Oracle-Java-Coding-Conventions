# Comments
Java programms can have kinds of comments: 1. implementation comments and 2. documentation comments. 

1. Implementation comments are those found in c/c++, which are delimited by /*...*/, and //.

2. Documentation comments (known as "doc comments") are those found in Java-only, and are delimited by /**...*/. These can be extracted to HTML files using the javadoc too. 

Implementation comments are mean for commenting out code or for comments about the
particular implementation. Doc comments are meant to describe the specification of the code,
from an implementation-free perspective. to be read by developers who might not necessarily
have the source code at hand.

Comments should be used to give overviews of code and provide additional information that is
not readily available in the code itself. Comments should contain only information that is
relevant to reading and understanding the program. For example, information about how the
corresponding package is built or in what directory it resides should not be included as a
comment.

Discussion of nontrivial or nonobvious design decisions is appropriate, but avoid duplicating
information that is present in (and clear from) the code. It is too easy for redundant comments
to get out of date. In general, avoid any comments that are likely to get out of date as the code
evolves.
Note: The frequency of comments sometimes reflects poor quality of code. When you feel
compelled to add a comment, consider rewriting the code to make it clearer.
Comments should not be enclosed in large boxes drawn with asterisks or other characters.
Comments should never include special characters such as form-feed and backspace.