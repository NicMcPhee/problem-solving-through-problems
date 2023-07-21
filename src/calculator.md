# Racket is a powerful, if slightly weird, calculator

```scheme
(+ 2 3)
```

Let's define a function that computes the Fibonacci numbers.

```scheme
(define (fib n)
    (if (< n 2)
        n
        (+ (fib (- n 1))
           (fib (- n 2)))))
```

```rust
fn fib(n: i64) -> i64 {
    if n < 2 then {
        n        
    } else {
        fib(n-1) + fib(n-2)
    }
}
```