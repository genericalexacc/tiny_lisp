# Tiny Lisp

This is a lisp interpreter that I wrote following along this book:
http://www.buildyourownlisp.com  


# Compile the interpreter
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

# Code Examples

Naive recursive Fibonacci function in tiny lisp
```common-lisp
(fun {fib n} {
  select
    { (== n 0) 0 }
    { (== n 1) 1 }
    { otherwise (+ (fib (- n 1)) (fib (- n 2))) }
})
```

Take n objects from a list
```common-lisp
(fun {take n l} {
  if (== n 0)
    {nil}
    {join (head l) (take (- n 1) (tail l))}
})
```

Apply a function to each element in list (map function)
```common-lisp
(fun {map f l} {
  if (== l nil)
    {nil}
    {join (list (f (fst l))) (map f (tail l))}
})
```
