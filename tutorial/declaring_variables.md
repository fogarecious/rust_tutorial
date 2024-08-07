# Declaring Variables

A variable is a kind of storage that we can put numbers, strings or other data types in it.
To declare a variable, we use `let`.
For exmple:

```rust
fn main() {
    let n = 1;
    println!("n is {}", n)
}
```

Output:

```text
n is 1
```

We can also store a string in a variable.

```rust
fn main() {
    let s = "Hello";
    println!("The string is \"{}\".", s);
}
```

Output:

```text
The string is "Hello".
```

We can compute and store a result of an expression before we print it out.

```rust
fn main() {
    let n = 11 * 19 + 3;
    println!("n = {}", n)
}
```

Output:

```text
n = 212
```

<!-- :arrow_right:  Next:  -->
If we declare a variable but not use it later as follows,

```rust
fn main() {
    let n = 1;
}
```

we will get a compiler warning when we execute `cargo build`.

```text
warning: unused variable: `n`
 --> src/main.rs:2:9
  |
2 |     let n = 1;
  |         ^ help: if this is intentional, prefix it with an underscore: `_n`
  |
  = note: `#[warn(unused_variables)]` on by default
```

We can put `_` before the variable name to fix this warning as suggested above.

```rust
fn main() {
    let _n = 1;
}
```


:blue_book: Back: [Table of contents](./../README.md)
