# Weekly Progress Report  
**Week:** 24 July 2025 – 30 July 2025  
**Author:** Ahaouariwadie (GitHub username)

---

## Summary of Activities

### Thursday, 24 July 2025
- Began reading [The Rust Programming Language](https://rust-book.cs.brown.edu/)
- Read the "Experiment Introduction", "The Rust Programming Language", and "Foreword"
- Completed the main "Introduction" chapter to understand the philosophy and safety principles of Rust
- Installed Rust using `rustup` and set up `cargo`, Rust’s package manager and build system

### Friday, 25 July 2025
- Worked through Chapter 1: *Getting Started*
  - 1.1. Installed Rust using `rustup` on Windows
  - 1.2. Wrote and compiled the first "Hello, World!" program using `rustc`
  - 1.3. Learned to use `cargo new`, `cargo build`, and `cargo run` to manage a Rust project
- Verified Rust installation with `rustc --version` and `cargo --version`

### Saturday, 26 July 2025
- Completed Chapter 2: *Programming a Guessing Game*
  - Wrote a number guessing game with:
    - Input handling using `io::stdin().read_line()`
    - Random number generation with the `rand` crate
    - Looping using `loop` and conditional logic with `if` / `match`
- Learned to use `Cargo.toml` to manage dependencies

### Sunday, 27 July 2025
- Studied Chapter 3: *Common Programming Concepts*
  - 3.1. Learned variable mutability (`let`, `mut`)
  - 3.2. Covered scalar and compound data types: integers, floats, booleans, chars, tuples, arrays
  - 3.3. Wrote and called functions with parameters and return values
  - 3.4. Understood how to use comments in Rust
  - 3.5. Practiced control flow with `if`, `else if`, `else`, and `loop`, `while`, `for`

### Monday, 28 July 2025
- Completed Chapter 4: *Understanding Ownership*
  - 4.1. Learned the ownership rules and how values move
  - 4.2. Studied references (`&`) and borrowing (`&mut`)
  - 4.3. Fixed ownership errors and understood the Rust borrow checker
  - 4.4. Used string slicing and learned about the slice type
  - 4.5. Reviewed ownership with code samples

### Tuesday, 29 July 2025
- Completed Chapter 5: *Using Structs to Structure Related Data*
  - 5.1. Defined and instantiated structs
  - 5.2. Built a struct-based program (e.g., to calculate the area of rectangles)
  - 5.3. Implemented methods using `impl` blocks and `self` references

### Wednesday, 30 July 2025
- Completed Chapter 6: *Enums and Pattern Matching*
  - 6.1. Defined enums with multiple variants (e.g., `Option`, custom types)
  - 6.2. Used `match` expressions to destructure and handle enum values
  - 6.3. Practiced concise control flow using `if let` and `let else`
  - 6.4. Completed Ownership Inventory #1 exercise

---

## Challenges & Notes
- The ownership model and borrowing rules were difficult at first but started to make sense after writing examples.
- Writing the guessing game gave a hands-on understanding of Rust’s strict compile-time checks.
- `cargo` made project management seamless and was easier to use than initially expected.

## Goals for Next Week
- Start working with the [CKB Contract Creation (CCC) Playground](https://docs.ckbccc.com/docs/ccc/)  
  → Use the interactive environment at [live.ckbccc.com](https://live.ckbccc.com/) to apply Rust skills in CKB contract development  
- Continue reviewing advanced Rust concepts when needed during the exercises

