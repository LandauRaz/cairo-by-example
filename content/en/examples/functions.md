---
title: "functions"
weight: 40
draft: false
---

A function is a unit of code that performs some logic. It is defined using the `fn` keyword, and the convention is to name functions using the 'snake_case' form. 


```rust {.codebox}
// This function returns an u32.
fn main() -> u32 {
    42
}

// This functions doesn't return anything.
fn inc_x(mut x: u32) {
    x = x + 1
}
```

Running this will yield:

```bash
Run completed successfully, returning [42]
```

Note that in Cairo, functions always return a value. When the function has no particular return value, it is common to return the unit type (`()`).
