# Printing Strings

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

The text put in quotes `""` is called a string.
`println!` helps us to print strings on the screen.

In addition, we can use `{}` to indicate a string that will be specified later.
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

We can format a printed text in the following way.

```rust
fn main() {
    println!("{}, {}!", "Hello", "world");
}
```

Output:

```text
Hello, world!
```

:arrow_right:  Next: [Printing Special Strings](./printing_special_strings.md)

:blue_book: Back: [Table of contents](./../README.md)
