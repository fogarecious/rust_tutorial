# Printing On Screen

We can use `println!` to print texts on the screen.
For example:

```rust
fn main() {
    println!("Hello");
}
```

This prints `Hello` on the screen.

```text
Hello
```

In addition, we can use `{}` to indicate a text that will be specified later.
For example:

```rust
fn main() {
    println!("{}", "Hello");
}
```

In the code, we tell the compiler that we need to print something, and this *something* is `Hello`.
The output is the same.

```text
Hello
```

The symbol `{}` is useful especially when we have more than one text.

```rust
fn main() {
    println!("{} {}", "Hello", "world");
}
```

This outputs:

```text
Hello world
```

We can format the text in the following way.

```rust
fn main() {
    println!("{}, {}!", "Hello", "world");
}
```

Output:

```text
Hello, world!
```

In addition to text, we can also specify numbers.

```rust
fn main() {
    println!("{}", 123);
}
```

Output:

```text
123
```

Or specify expressions.

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

<!-- :arrow_right:  Next:  -->

:blue_book: Back: [Table of contents](./../README.md)
