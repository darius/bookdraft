When you program, how many layers of programs sit between you and your
hardware? These programs together do marvels, yet nobody understands
them all. When Steve Wozniak designed and built his Apple ][ almost
single-handed, he assembled the ROMs byte-by-byte himself; some of the
users studied the system to the same degree. It's common to feel we've
lost something since then.

XXX expand with Kragen's tol Code Reuse Considered Harmful, etc.

In this book I'm going to build a whole programming environment on a
base of simple primitives. I'll do it more than once, to try to learn
to do it well. I'll program from the perspective that we program to
learn and to explain what we've learned, not just to make a computer
do things. We'll work in a variation of Donald Knuth's idea of
literate programming; the systems built will try to support that style
of work, and take the idea further to bring a literate perspective to
a running, self-hosting system, not just static printouts.

Let's start Forth.

XXX build on MMIX instead of C?
      
      (in forth.c)
      #include <stdio.h>
      #include <stdlib.h>

Our Forth dialect should support our goal of literate programming. 

      int main () {
          return 0;
      }
