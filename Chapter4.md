# Chapter 4 Exercises

## Exercise 1

Extend the definitions of `kar` and `kdr` (frame 4.42) so they work with arbirary
Pairs (instead of just for `Pair Nat Nat`).

frame 4.42:

```pie
(define kar
  (lambda (p)
    (elim-Pair
      Nat Nat
      Nat
      p
      (lambda (a d)
        a))))

(define kdr
  (lambda (p)
    (elim-Pair
      Nat Nat
      Nat
      p
      (lambda (a d)
        d))))
```

## Exercise 2

Define a function called compose that takes (in addition to the type
arguments A, B, C) an argument of type `(-> A B)` and an argument of
type `(-> B C)` that and evaluates to a value of type `(-> A C)`, the function
composition of the arguments.
