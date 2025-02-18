---
title: "assert"
weight: 20
draft: false
---
To make sure things work, we use `assert`:

```rust {.codebox}
fn main() {
    assert(4 != 2, "Oops!");
}
```

The first argument of `assert` is the condition we want to check, and the second is a message we will see on the console if the condition is false.

Running this will yield:

```bash
Run completed successfully, returning []
```

Try changing it so that the test fails.
