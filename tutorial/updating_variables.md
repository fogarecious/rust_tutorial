# Updating Variables

By default, variables cannot change their values.
For example:

```rust
let n = 1;
n = 2;
```

We will get a compiler error when we run `cargo build` with the code.

```text
error[E0384]: cannot assign twice to immutable variable `n`
 --> src/main.rs:3:5
  |
2 |     let n = 1;
  |         -
  |         |
  |         first assignment to `n`
  |         help: consider making this binding mutable: `mut n`
3 |     n = 2;
  |     ^^^^^ cannot assign twice to immutable variable
```

To overwrite the value of a variable, we can use `mut` in the following way.

```rust
let mut n = 1;
println!("{}", n);
n = 2;
println!("{}", n);
```

`mut` allows a variable to update its value.
We can see from the output that the value of `n` changes.

Output:

```text
1
2
```

<!-- :arrow_right:  Next:  -->

:blue_book: Back: [Table of contents](./../README.md)
