# Printing Numbers

In addition to strings, we can also print numbers that are specified by `{}`.
For example:

```rust
fn main() {
    println!("{}", 123);
}
```

Output:

```text
123
```

The numbers can be replaced with arithmetic expressions.

```rust
fn main() {
    println!("{}", 2 + 4 * 3);
}
```

Output:

```text
14
```

The expressions can be combined with a formatted text.

```rust
fn main() {
    println!("{} x {} = {}", 14, 9, 14 * 9);
}
```

Output:

```text
14 x 9 = 126
```

:arrow_right:  Next: [Declaring Variables](./declaring_variables.md)

:blue_book: Back: [Table of contents](./../README.md)
