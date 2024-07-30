# The First Project

To create a [Rust](https://www.rust-lang.org/) project, we use the command below:

```sh
cargo new my_project
```

where `my_project` is the name of our project.

This command creates a folder `my_project`.
There are two items in folder `my_project`, `Cargo.toml` and `src`.
`Cargo.toml` is a file for package management.
`src` is a folder that contains all our source code files, usually with names end with `.rs`.

There is a file, `main.rs`, created in folder `src`.
The file has the default function.
We can execute this function by the commands below:

```sh
cd my_project
cargo run
```

`cargo run` compiles and runs our program.
We can run `cargo run` anywhere in folder `my_project`.
Running the program gives us the following output:

```text
Hello, world!
```

Sometimes, we only need to compile the program but not actually run it.
For example, when we want to make sure that the program has no compile errors.
In this case, we can use the command below:

```sh
cargo build
```

Finally, when we are ready to publish our program and need our program to be compiled in the optimal way, we can use the command below:

```sh
cargo build --release
```

We can find the result executables in folder `target`, which is in folder `my_project`.
If we build the project with `--release` flag, we can find the executable in folder `target/release`.
Otherwise, we can find it in folder `target/debug`.

<!-- :arrow_right:  Next:  -->

:blue_book: Back: [Table of contents](./../README.md)
