# Explanation Of The First Program

Let's look at `src/main.rs`.

```rust
fn main() {
    println!("Hello, world!");
}
```

The file contains a function `main`, which is the starting point of the program.
Our code will be placed between `{` and `}`.
The code usually consists of statements, each of which ends with `;`.
In this code, there is only one statement, `println!("Hello, world!");`.
`println!` helps us printing a string on the screen.

In addition, white spaces that do not change the meaning of the code will be ignored by the compiler.
So, we can also write the same code in the following way.

```rust
fn main(){println!("Hello, world!");}
```

<!-- :arrow_right:  Next:  -->

:blue_book: Back: [Table of contents](./../README.md)
