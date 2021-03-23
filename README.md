# Data Lab

This repository contains the solution code for the first of 11 individual labs
in the CS:APP (3e) course: Data Lab.

## Overview

The project implements seven functions on basic bit manipulation and both
integer/floating point manipulation at the lowest level. These functions are
split into portions; Each portion and their individual functions is listed in
more detail below.

## Testing

The `./dlc` Data Lab Compiler handles checking for correctness of code. In order
to utilize this, use the following command:

```
  unix> ./dlc bits.c
```

To count the number of operations within code, use the following:

```
  unix> ./dlc -e bits.c
```

Finally, to test the validity of functions, use the `./btest` testing scripts.

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

## 1st Portion

### Function 1.1: `bitXor`

```c
int bitXor(int x, int y);
```

Taking two inputs, this function outputs the value of `x XOR y`.

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
