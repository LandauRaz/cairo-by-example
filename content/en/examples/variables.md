---
title: "variables"
weight: 30
draft: false
---

To store data in variables use the `let` keyword. If you need to change the stored data, the variable must be marked mutable using `let mut`:

```rust {.codebox}
fn main() {
    let immutable_var: felt252 = 17;
    // immutable_var = 38;  <-- fails to compile

    // but this is legal:
    let mut mutable_var: felt252 = immutable_var;
    mutable_var = 38;

    assert(mutable_var != immutable_var, 'mutable equals immutable');
}

#[test]
fn test_main() {
    main();
}
```

Running this will yield:

```bash
Run completed successfully, returning []
```

Try changing it so that the test fails.
