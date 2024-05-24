## 02-Hellocargo

### Introduction to Cargo
Cargo is Rust’s build system and package manager. It simplifies managing Rust projects by handling tasks such as building code, downloading dependencies, and compiling those dependencies.

### Checking Cargo Installation
Ensure Cargo is installed by running:
```bash
$ cargo --version
```
If installed, this will return the version number. If not, refer to the installation documentation for guidance.

### Creating a New Project
To create a new project with Cargo, run the following commands:
```bash
$ cargo new hello_cargo
$ cd hello_cargo
```
This sets up a new project directory named `hello_cargo` with a basic "Hello, world!" program.

### Project Structure
Cargo creates two main files:
- `Cargo.toml`: The project’s configuration file.
- `src/main.rs`: The main source file containing the code.

#### `Cargo.toml`
This file contains metadata about your project. Example:
```toml
[package]
name = "hello_cargo"
version = "0.1.0"
edition = "2021"

[dependencies]
```

#### `src/main.rs`
This file contains the Rust code:
```rust
fn main() {
    println!("Hello, world!");
}
```

### Building and Running the Project
To build and run your Cargo project, use the following commands:
```bash
$ cargo build
$ ./target/debug/hello_cargo  # or .\target\debug\hello_cargo.exe on Windows
```
Or, more conveniently:
```bash
$ cargo run
```
Cargo also supports `cargo check` for quickly checking if the code compiles without producing a binary:
```bash
$ cargo check
```

### Building for Release
For an optimized build, use:
```bash
$ cargo build --release
```
This creates an optimized executable in the `target/release` directory.

### Summary
In this chapter, you've learned how to:
- Create a new Rust project with Cargo.
- Understand the basic structure of a Cargo project.
- Build and run your project.
- Use Cargo for managing dependencies and optimizing builds.

### Quiz

**Question:**
Say you just downloaded a Cargo project, and then you run `cargo run` at the command-line. Which statement is NOT true about what happens next?

**Answer:**
Cargo watches for file changes and re-executes the binary on a change.
