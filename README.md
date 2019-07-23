Do you ever find yourself wanting to use scheme programs in Common Lisp? 

scheme2common-lisp can help ease the nightmare of porting scheme programs to Common Lisp. 
scheme2common-lisp contains scheme functions implemented in Common Lisp, to make copy-pasting the scheme programs into Common Lisp as smooth as possible.

# How To

1. You want to use scheme code in Common Lisp
2. Copy and paste the scheme code you want to use into your common lisp package
3. Use the ```:scheme2common-lisp``` package in the package you want to run the scheme code in.
4. Smooth out any inconsistencies....
5. Profit!

# Technical details 

Some Scheme functions are Common Lisp functions under a different name. 
Some Scheme primitives require more complex Common Lisp Implementations, like ```named-let``` and ```letrec```.

```(use-package :scheme2common-lisp)```

Implemented functions:

```
atom?
symbol?
pair?
null?
eq?
equal?
integer?
for-each
assq
reverse!
remainder
modulo
quotient
assv
display
eqv?
list-ref
list-tail
memq
memv
newline
set-car!
set-cdr!
vector-ref
vector-set!
string-ref
string-set!
vector-length
number?
string?
list?
string-append
number->string
symbol->string
char->integer
integer->char
list->string
string-length
pp
set!
begin
named-let
make-vector
+true+
+false+
letrec
call/cc
open-input-file
close-input-port
```

# Use Cases:
![Lisp In Small Pieces](https://github.com/gmasching/lisp-in-small-pieces)

![Scheme2LLVM](https://github.com/gmasching/scheme2llvm)
