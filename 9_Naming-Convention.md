# Naming Convetions

Naming conventions make programs more understandable by making them easier to read. They can also give information about the function of the identifier.

| Identifier Type | Rules for Naming | Examples |
|---|---|---|
|Classes|Class name should be nouns, in *mixed case* with the first letter of each internal word capitalized. Keep it simple and descriptive Use whole words- avoid acronyms and abbreviations(unless it more widely used than long form, such URL or HTML)|```class RasterSprite```|
|Interfaces|Interface names should be capitalized like class name|```interface RasterDelegate```|
|Methods|Methods should be verbs, in mixed case with the first letter lowercase, with the first letter of each internal word capitalized.|```getBackground()```|
|Variables|Except for variables, all instances, class, and class constants are in mixed case with a lower-case first letter. Internal words start with capital letters. |``` int i; float myWidth;```|
|Constants|The names of variables declared class constants and of ANSI constants should be all uppercase with words separated by under-scores. (ANSI constants should be avoided, for ease of debugging.)|```int MIN_WIDTH = 4; int MAX_WIDTH = 999; int GET_THE_CPU = 1```|

**Note:** 
- *Variable names should be short yet meaningful. The choice of a variable name should be mnemonic- that is, designed to indicate to the casual observer the intent of its use.*
- *One-character variable names should be avoided except for temperory "throwway" variables.*
- *Common names for temperory variables are:*
*a) Integers: i, j, k, m and n*
*b) Characters: c, d, and e*