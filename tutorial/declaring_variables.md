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

:blue_book: Back: [Table of contents](./../README.md)
