## Source files to compile agepro.exe

-   **C code files**
    -   agepro.c — *the main C code*
    -   ranx.c — *generates random Uniform(0,1) variates*
    -   boxmuller.c — *generates pairs of random Normal(0,1) variates*
    -   util.c — *utility functions*
-   **C header files**
    -   agepro.h
    -   ranx.h
    -   util.h

## Steps to compile agepro.exe using a C compiler

1.  Compile object files for ranx.c, boxmuller.c, and util.c using the gcc compiler\
    gcc -c ranx.c\
    gcc -c boxmuller.c\
    gcc -c util.c

2.  Compile agepro.c, link object files, and name the executable agepro.exe\
    gcc -o agepro.exe ranx.o boxmuller.o util.o agepro.c
