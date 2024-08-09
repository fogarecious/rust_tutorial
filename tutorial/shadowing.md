# Shadowing

[Rust](https://www.rust-lang.org/) allows developers to re-use a name of a variable.
For example:

```rust
let x = 1;
let x = 2;
```

In the example, symbol `x` is used for declaring a variable and then it is re-used for declaring another variable.
This type of variable declaration is called *shadowing*.

Shadowing is useful when we have nested scopes.

```rust
let x = 1;
let y = 2;
{
    let x = 3;
    println!("x = {}", x);
    println!("y = {}", y);
}
println!("x = {}", x);
println!("y = {}", y);
```

Output:

```text
x = 3
y = 2
x = 1
y = 2
```

`{}` opens a new scope.
We can re-use a variable name in the inner scope while leaving the variable in the outer scope unchanged.

Another reason to use shadowing is to change the type of a variable.

```rust
let x = "one";
let x = 1;
```

This is helpful when the program becomes complicated.

<!-- :arrow_right:  Next:  -->

:blue_book: Back: [Table of contents](./../README.md)
