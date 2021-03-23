# Data Lab

This repository contains the solution code for the first of 11 individual labs
in the CS:APP (3e) course: Data Lab.

## Overview

The project implements seven functions on basic bit manipulation and both
integer/floating point manipulation at the lowest level. These functions are
split into portions; Each portion and their individual functions is listed in
more detail below.

## Testing

To test the validity of functions, use the `./btest` testing scripts.

```
  unix> ./btest -h
  Usage: ./btest [-hg] [-r <n>] [-f <name> [-1|-2|-3 <val>]*] [-T <time limit>]
    -1 <val>  Specify first function argument
    -2 <val>  Specify second function argument
    -3 <val>  Specify third function argument
    -f <name> Test only the named function
    -g        Format output for autograding with no error messages
    -h        Print this message
    -r <n>    Give uniform weight of n for all problems
    -T <lim>  Set timeout limit to lim
```

There is a separate tester called `./dlc` for testing validity of the code files
themselves; However, I have not successfully executed this validity checker on
my end.

## 1st Portion

### Function 1.1: `bitXor`

```c
int bitXor(int x, int y);
```

Taking two inputs, this function outputs the value of `x XOR y`. This function
may only use the logical AND `&` and logical NOT `~` operators.

From a circuit standpoint, the XOR function is represented by the following
excitation equation:

```
x XOR y = (x | y) & (~x | ~y)
```

We can transform this into the following:

```
x XOR y =  ( x |  y) &  (~x | ~y)       Original
x XOR y =  ( x |  y) & ~( x &  y)       Remove a ~ from second term
x XOR y = ~(~x & ~y) & ~( x &  y)       Remove a ~ from first term
```

This representation is now completely in AND and NOT operators.

# License TL;DR

This project is distributed under the MIT license. This is a paraphrasing of a
[short summary](https://tldrlegal.com/license/mit-license).

This license is a short, permissive software license. Basically, you can do
whatever you want with this software, as long as you include the original
copyright and license notice in any copy of this software/source.

## What you CAN do:

-   You may commercially use this project in any way, and profit off it or the
    code included in any way;
-   You may modify or make changes to this project in any way;
-   You may distribute this project, the compiled code, or its source in any
    way;
-   You may incorporate this work into something that has a more restrictive
    license in any way;
-   And you may use the work for private use.

## What you CANNOT do:

-   You may not hold me (the author) liable for anything that happens to this
    code as well as anything that this code accomplishes. The work is provided
    as-is.

## What you MUST do:

-   You must include the copyright notice in all copies or substantial uses of
    the work;
-   You must include the license notice in all copies or substantial uses of the
    work.

If you're feeling generous, give credit to me somewhere in your projects.
