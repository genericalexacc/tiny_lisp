# Tiny Lisp

This is a lisp interpreter that I wrote following along this book:
http://www.buildyourownlisp.com  


# Usage
To compile run
```console
foo@bar:~$ cc -std=c99 -Wall tlisp.c mpc.c -ledit -lm -o tiny_lisp
```

Then to run the REPL:
```console
foo@bar:~$ ./tiny_lisp
```

or to run a file

```console
foo@bar:~$ ./tiny_lisp std.tlsp
```
