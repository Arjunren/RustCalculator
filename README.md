# Rust CLI Calculator

## Description
A lightning-fast, command-line calculator written in Rust. This lightweight utility performs standard arithmetic operations—addition, subtraction, multiplication, and division—directly from your terminal. Built with memory safety and zero-cost abstractions, it offers robust error handling for invalid inputs and division by zero. Fast and simple.

## Requirements
- Rust and Cargo (Install via [rustup](https://rustup.rs/))

## Setup
Initialize a new Cargo project and replace the contents of `src/main.rs` with the provided code.
```bash
cargo new rust_calculator
cd rust_calculator
```

## Usage
Run the calculator using Cargo. Provide two numbers and an operator (`+`, `-`, `*`, `x`, `/`) separated by spaces. 

*Note: In many Unix shells, the `*` character acts as a wildcard. Escape it using `\*` or use `x` for multiplication.*

### Examples

**Addition:**
```bash
cargo run -- 15.5 + 4.5
# Output: 15.5 + 4.5 = 20
```

**Subtraction:**
```bash
cargo run -- 100 - 42
# Output: 100 - 42 = 58
```

**Multiplication:**
```bash
cargo run -- 7 \* 8
# Output: 7 * 8 = 56

cargo run -- 7 x 8
# Output: 7 x 8 = 56
```

**Division:**
```bash
cargo run -- 25 / 5
# Output: 25 / 5 = 5
```

## Building for Production
To compile an optimized, standalone executable:
```bash
cargo build --release
```
The compiled binary will be available at `./target/release/rust_calculator`.
