# Hello, World!

- Rust files always end with the `.rs` extension.
- Use an underscore to separate words.
- The `main` function is always the first code that runs in every executable Rust program.
- Place the opening curly bracket on the same line as the function declaration with one space in between.
- The Rust team has included a tool named `rustfmt`. Use it like `rustfmt main.rs` to apply formatting to your Rust code.
- Rust style is to indent with four spaces, not a tab.
- Using a `!` (in this case `println!`) means you're calling a Macro. Macros are different than functions and don't always follow the same rules as functions.
- Most lines of Rust code end with a semicolon.
- `rustc sourcefile.rs` will compile your code.
- After compiling, Rust outputs a binary executable. 
- Rust is an ahead-of-time complied language, you can compile a program and give the executable to someone else, and they can run it without having Rust installed.