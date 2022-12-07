# Hello, cargo!

- `cargo` is Rust's build system and package manager. 
- use `cargo new project_name` to create a new project.
- `Cargo.toml` contains project configuration details such as packages (known as crates) and more.
- `cargo build` will compile your project.
- `cargo run` will compile and run. If `cargo` doesn't detect any code modifications, a build will not happen.
- `cargo` stores the results of the build in the `target/debug` directory.
- `cargo check` will check your code to make sure it compiles but doesn't produce an executable.
- Run `cargo check ` periodically as your write your code to make sure it complies.
- `cargo build --release` compiles with optimizations and creates an executable in `target/release`