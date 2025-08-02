# Curdler
A basic C compiler for the pARMesan architecture.

## Compiler Structure
The compiler will consist of 3 stages:
1. lexer
    - tokenizes the C file
2. parser
    - parses the stream of tokens and constructs an abstract syntax tree (AST)
3. codegen
    - use the AST to generate parmesan wheel file

In the future, support for a simple preprocessor could be made.

## Features Supported
Due to the limitations of the pARMesan architecture only a small subset of C features will be supported.

### Data Types
Data types supported are `char` and `short`, defined to be 1 byte and 2 bytes respectively.
Pointers to these data types are also allowed, pointers are 2 bytes in size.

### Control Flow
The supported control flow blocks are `if` statements, `labels` and `goto` statements, and `for` & `while` loops.
Functions can be created and call like normal in C.

### Arithmetic
Obviously we can do basic math.

### Bit Manipulation
You can perform `&`, `|`, and `^` (xor); using those symbols.

## More Features?
As this whole project is under development, you can be sure that more features can be added.
Stuff like:
- structs
- some other C features that I can't think of right now.
