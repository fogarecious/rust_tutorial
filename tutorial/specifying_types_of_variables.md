# Specifying Types Of Variables

By default, an integer will be stored in type `i32`, which is a signed 32-bit integer.
We can change types by `:` when we declare variables.
For example, we can declare an unsigned 32-bit integer that has value `1`.

```rust
let n: u32 = 1;
```

Since the variable is of type `u32`, it will get a compiler error if its value exceeds the range of `u32` as follows.

```rust
let n: u32 = 4294967296;
```

This gives the following error when we execute `cargo build`.

```text
error: literal out of range for `u32`
 --> src/main.rs:2:18
  |
2 |     let n: u32 = 4294967296;
  |                  ^^^^^^^^^^
  |
  = note: the literal `4294967296` does not fit into the type `u32` whose range is `0..=4294967295`
  = note: `#[deny(overflowing_literals)]` on by default
```

We can change the type, say `u64`, to have larger ranges.

```rust
let n: u64 = 4294967296;
```

Now, there is no compiler errors.

We will explain more about types in detail later.

<!-- :arrow_right:  Next:  -->

:blue_book: Back: [Table of contents](./../README.md)
