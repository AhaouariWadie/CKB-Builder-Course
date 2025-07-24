# Weekly Progress Report  
**Week:** 17 July 2025 – 23 July 2025  
**Author:** Ahaouariwadie (GitHub username)

---

## Summary of Activities

### Thursday, 17 July 2025
- Installed and initialized [Rustlings](https://github.com/rust-lang/rustlings) to practice Rust fundamentals.
- Reviewed the purpose of `rustlings watch` to automatically re-run exercises as they are saved.
- Completed the `variables` and `functions` exercises, learning Rust’s:
  - `let`, `mut`, and variable shadowing.
  - Function definitions and return values without explicit `return`.

### Friday, 18 July 2025
- Worked through the `if` and `primitive_types` exercises.
- Practiced:
  - Conditional expressions using `if` as an expression.
  - Scalar types: integers, floats, booleans, and characters.
  - Tuple and array destructuring in `primitive_types`.

### Saturday, 19 July 2025
- Focused on `vecs` and `strings` exercises:
  - Used `.push()`, `.pop()`, indexing, and `.len()` for vectors.
  - Understood UTF-8 encoding in Rust strings and methods like `.push_str()` and `.len()`.
  - Accessed elements with indexing and slicing.
  - Practiced borrowing (&vec) and mutable references (&mut vec) in loops.


### Sunday, 20 July 2025
- eviewed all prior concepts, Focused on clarifying: 
  - Difference between stack and heap.
  - Ownership implications in arrays and vectors.
  - When to prefer cloning vs borrowing.


### Monday, 21 July 2025
- Studied ownership concepts in Rust as an introduction to memory safety.
- Started the `06_move_semantics` block of exercises.
- Learned:
  - Ownership transfer (moves) between functions and variables.
  - Borrowing via references and the `&mut` keyword for mutable borrowing.

### Tuesday, 22 July 2025
- Continued `move_semantics` exercises.
- Practiced correcting common mistakes:
  - Using `clone()` vs borrowing to avoid move errors.
  - Modifying data with mutable references inside functions.

### Wednesday, 23 July 2025
- Completed the final exercises in the `move_semantics` module.
- Summarized key Rust concepts:
  - The rules of ownership and borrowing.
  - Difference between stack-allocated and heap-allocated values.
- Prepared for upcoming modules on traits and lifetimes.

---

## Challenges & Notes
- Understanding the difference between moving and borrowing was initially confusing but improved with practice.
- Rustlings’ auto-feedback made it easier to iterate quickly on errors.
- Matching Rust’s strict compiler rules helped reinforce memory-safe patterns.

## Goals for Next Week
- Begin exploring Rust traits and implement traits for custom types.
- Complete exercises on lifetimes and closures.
- Compare memory safety approaches in Rust and JavaScript for smart contract development.
