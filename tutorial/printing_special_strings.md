# Printing Special Strings

Sometimes, we want to print symbol `"`.
In this case, we have to type `\` before `"`.
For example:

```rust
fn main() {
    println!("\"");
}
```

Output:

```text
"
```

There are other special symbols such as `{`, `}` and `\` that require special forms to print them.

```rust
fn main() {
    println!("{{");
    println!("}}");
    println!("\\");
}
```

Output:

```text
{
}
\
```

These symbols may look like this when they are combined with other texts:

```rust
fn main() {
    println!("{{}} is a pair of \"braces\". \\(o.o)/");
}
```

Output:

```text
{} is a pair of "braces". \(o.o)/
```

:arrow_right:  Next: [Printing Numbers](./printing_numbers.md)

:blue_book: Back: [Table of contents](./../README.md)
