# Myau!

#### All projects in this repositories were made as part of my MIPT programming courses.
They laid foundation of my knowledge, small description of most valuable and inetresting ones you can find here.
 
 ### C projects:
  - Pr.3-Soft_CPU:
  
    My own assembler language and the program that compiles it are
    implemented here. Text on my assembler is converted to a binary file. Then
    another program is reading a binary file and executing commands. Both
    programs and main header are using preprocessor code generation, so it’s very
    easy to expand the list of commands, and code is highly readable. 
  - Pr.6-Differentiate:
  
    It’s a program that differentiates expressions with variables and some
    functions. It is generating a LaTeX file as a result. Expression is parsed into a
    tree with a recursive descent method. For differentiating I wrote DSL, so the
    code is very easy to understand. There is also a simplification of tree and autogeneration of an output LaTeX file.

  ### ASM projects:
  - MPrintf:

    It’s my realization of printf, written in x86_64 NASM. It can understand 6
    specifiers (%c, %s, %d, %b, %o, %x) and %%, if you want to print a percent
    symbol. To decide which specifier was used, the MPrintf program is using
    JumpTable, so it’s fast. I also implemented buffer overflow protection. And
    there are 2 more files, where you can find calling printf from the NASM
    program and MPrintf from C program.
  - Mandlebrot Set:

    It’s a program that draws a Mandelbrot set, using SDL library. It is
    implemented with 3 modes – drawing, not optimized and optimized. In the
    first mode you can see a picture of set and fps, two other modes don’t draw
    a picture but show you only fps. Not optimized version counts each point
    separately, while the optimized version uses Intel Intrinsics for counting 4
    points at a time. In drawing mode the best version is called (of course with
    SSE & AVX optimization it gets faster). There is also an algorithmic
    optimization, which is based on the idea that we can draw whole rectangles
    of points in one colour.
