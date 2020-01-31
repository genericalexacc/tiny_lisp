# Tiny Lisp

This is a lisp interpreter that I wrote following along this book:
http://www.buildyourownlisp.com  


# Usage
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
