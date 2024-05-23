# 01-Helloworld

## Introduction
Welcome to your first Rust program! In this guide, we'll walk you through writing a simple "Hello, World!" program in Rust and explain the basics to get you started.

## Setting Up Your Project

### Creating a Project Directory
First, let's create a directory to store your Rust code. Open your terminal and enter the following commands:

For Linux, macOS, and PowerShell on Windows:
```bash
$ mkdir ~/projects
$ cd ~/projects
$ mkdir hello_world
$ cd hello_world
```

For Windows CMD:
```cmd
> mkdir "%USERPROFILE%\projects"
> cd /d "%USERPROFILE%\projects"
> mkdir hello_world
> cd hello_world
```

### Writing Your First Rust Program
Next, create a new source file named `main.rs`. Open the file and enter the following code:

```rust
fn main() {
    println!("Hello, world!");
}
```

### Running Your Program
Save the file and compile it using the Rust compiler. In your terminal, navigate to the `~/projects/hello_world` directory and enter the following commands:

For Linux or macOS:
```bash
$ rustc main.rs
$ ./main
```

For Windows:
```cmd
> rustc main.rs
> .\main.exe
```

You should see the output:
```
Hello, world!
```

Congratulations! You've written and run your first Rust program.

## Understanding the Code

### The `main` Function
The `main` function is the entry point of every executable Rust program:
```rust
fn main() {
    // function body
}
```
- `fn main() {}` declares a function named `main` with no parameters and no return value.
- The function body is enclosed in curly brackets `{}`.

### Printing to the Console
```rust
println!("Hello, world!");
```
- `println!` is a macro that prints the string `Hello, world!` to the console.
- Strings in Rust are enclosed in double quotes `"`.
- Lines of code in Rust end with a semicolon `;`.

### Compilation and Execution
Rust is an ahead-of-time compiled language, meaning you compile the code before running it. This process produces a binary executable.

### Compiling Your Code
To compile your program, use the `rustc` command:
```bash
$ rustc main.rs
```
This creates an executable file (`main` on Linux/macOS, `main.exe` on Windows).

### Running the Executable
Run the compiled executable:
```bash
$ ./main  # or .\main.exe on Windows
```



