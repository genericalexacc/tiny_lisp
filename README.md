# Tyson Lisp
Tyson Lisp

![Image of Yaktocat](https://upload.wikimedia.org/wikipedia/commons/f/f2/Mike_Tyson_Portrait.jpg)

This is the result of the Build your Lisp book.  
http://www.buildyourownlisp.com  
It is a lisp built from scratch in C.  
It is not very different at all from the lisp in the book but it is my own.  

To compile run
```console
foo@bar:~$ cc -std=c99 -Wall tyson.c mpc.c -ledit -lm -o tyson
```

Then to run the REPL:
```console
foo@bar:~$ ./tyson
```

or to run a file

```console
foo@bar:~$ ./tyson std.tlsp
```