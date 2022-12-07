# Guessing game

I ran into an issue with the `rust-analyzer` today. I was getting `rust-analyzer failed to discover workspace` message.

Turns out it's because I'm using WSL to work with Rust. `rustup` was installed WSL.

Issue resolved by installing the WSL VS Code extension and opening my projects from WSL terminal with `code .` command. Thanks to this GitHub issue [comment](https://github.com/rust-lang/rust-analyzer/issues/7268#issuecomment-1236513645)

## Notes

- Rust has a set of items (prelude) defined in the standard library `std`. If a type you want isn't in the prelude, you'll have to bring it into scope explicitly with a `use` statement. 
` Variables by default are immutable. You;ll have to add `mut` before the variable name to make it mutable. 
- An associated function (`::` syntax) is a function that's implemented on a type.
- `&` indicates that an argument is a reference. References give you a way to let multiple parts of your code access one piece of data without needing to copy that data into memory multiple times. Like variables, they are immutable by default.
- It's best practice to introduce a newline and other whitespace to help break up long lines when you call a method with the `.method_name()` syntax.
- An `enumeration` (enum) is a type that can be in one of multiple possible states (variant).
- `Result` is an `enumeration` with variants `Ok` and `Err` and it's purpose is to encode error-handling information. 
- `crates` are collections of Rust source code files.
    - a binary crate is an executable
    - a library crate contains code intended to be used in other programs and can't be executed on its own.
- Cargo fetches latest version of dependencies in `Cargo.toml` from Crates.io
- `Cargo.lock` is a mechanism that ensures you can rebuild the same artifact every time your code is built. 
- When you build your project for the first time, Cargo figures out all the versions of the dependencies needed and writes them to `Cargo.lock`. Subsequent builds will use this file instead of figuring out versions again. It's often checked into source control with the rest of code. 
- a `match` expression is made up of arms, each arms consists of a pattern to match against and the code that should be run if the value given to `match` fits the arm's pattern.
- Rust has a strong, static type system. It also has type inference. Use a `:` after a variable name to annotate it's type.
- Shadowing lets us reuse variables rather than creating new ones. Often used when you want to covert a value from one type to another. 
- `_` is a catchall value